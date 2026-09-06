# Linux-Assessment
This repo contains TASKS ONLY. No command names, command options, or solutions are intentionally given as hints. Use your Linux knowledge, manual pages, built-in help, and lab experimentation to discover the commands.

# LINUX DEVOPS PRACTICAL PRACTICE — 300 TASKS

## TASK-ONLY WORKBOOK

This file contains TASKS ONLY.
No command names, command options, or solutions are intentionally given as hints.
Use your Linux knowledge, manual pages, built-in help, and lab experimentation to discover the commands.

For every mission, record separately: command discovered, important output, diagnosis, action, and verification.

## 1. FILESYSTEM HIERARCHY & LINUX BASICS

1. Find the username of the account currently running your shell.  root@ip-172-31-28-15:~# whoami
root

3. Find the absolute path of your current working directory.  root@ip-172-31-28-15:~/command1# pwd
/root/command1

4. Find the Linux kernel release currently running on the server.  root@ip-172-31-28-15:~/command1# uname -r
7.0.0-1011-aws

5. Find the Linux system/kernel name.  root@ip-172-31-28-15:~/command1# uname -s
Linux

6. Display complete kernel and system information.   uname -a
Linux ip-172-31-28-15 7.0.0-1011-aws #11-Ubuntu SMP PREEMPT Thu Aug  6 15:41:35 UTC 2026 x86_64 GNU/Linux

7. Identify the Linux distribution and release version.

8. Find the server's configured hostname. root@ip-172-31-28-15:~/command1#. hostname
ip-172-31-28-15

9. Identify whether the server is 32-bit or 64-bit.   name -m
x86_64

10. Display the current date and time.    root@ip-172-31-28-15:~/command1# date
Sat Sep  5 16:09:01 UTC 2026

11. Find how long the server has been running and its current load averages.   root@ip-172-31-28-15:~/command1# uptime
 16:09:43 up 19 min,  1 user,  load average: 0.00, 0.00, 0.00

12. Identify the CPU model used by the server. lscpu
Model name:                Intel(R) Xeon(R) Platinum 8259CL CPU @ 2.50GHz

14. Find the number of logical CPUs available.

15. Display total, used, free, and available memory.  free -m
               total        used        free      shared  buff/cache   available
Mem:             908         545          89           7         388         362

16. Display disk space usage for all mounted filesystems in a human-readable format. df -h
Filesystem       Size  Used Avail Use% Mounted on
/dev/root        6.7G  4.5G  2.2G  68% /
tmpfs            455M     0  455M   0% /dev/shm
tmpfs            182M  892K  181M   1% /run
efivarfs         128K  3.3K  120K   3% /sys/firmware/efi/efivars
tmpfs            455M  4.8M  450M   2% /tmp
none             1.0M     0  1.0M   0% /run/credentials/systemd-journald.service
none             1.0M     0  1.0M   0% /run/credentials/systemd-resolved.service
/dev/nvme0n1p13  989M  163M  760M  18% /boot
/dev/nvme0n1p15  105M  6.3M   99M   7% /boot/efi
none             1.0M     0  1.0M   0% /run/credentials/systemd-networkd.service
none             1.0M     0  1.0M   0% /run/credentials/getty@tty1.service
none             1.0M     0  1.0M   0% /run/credential

17. Explore the system configuration directory and identify at least five important configuration files.

18. Explore the system log directory and identify the major system/service logs present.

19. Identify the home directories belonging to normal users.

20. Find the home directory used by the superuser account.

21. Inspect the temporary-file directory and identify its purpose.

22. Identify where common user-space programs and libraries are stored.

23. Identify the standard location used for optional third-party applications.

24. Explore device files and identify examples representing disks or terminals.

25. Explore the process-information virtual filesystem and identify directories belonging to running processes.

26. Explore the kernel/device virtual filesystem and identify information about devices.

27. Explore runtime state files and identify examples of PID files or sockets.

28. Locate the server-side remote-login configuration directory.

29. Locate the current user's remote-login configuration and key directory.

30. Find the executable path of a common command available on the server.

31. Read the built-in documentation for a common Linux command and identify five useful options.

32. Create a short system-information report containing the hostname, kernel, uptime, CPU, memory, and disk information.

## 2. FILE & DIRECTORY MANAGEMENT

31. Create a file named `app.log`.  touch app.log

32. Create a directory named `devops`. mkdir devops

33. Create the nested directory structure `devops/project/src` in one operation.  mkdir -p devops/project/src

34. Create `logs`, `scripts`, and `backup` inside the `devops` directory. mkdir logs
root@ip-172-31-28-15:~/devops# mkdir backup
root@ip-172-31-28-15:~/devops# mkdir scripts
root@ip-172-31-28-15:~/devops# ls
backup  logs  project  scripts

35. Create `app.log`, `error.log`, and `access.log` inside `devops/logs`.  root@ip-172-31-28-15:~/devops/logs# touch app.log
root@ip-172-31-28-15:~/devops/logs# touch error.log. root@ip-172-31-28-15:~/devops/logs# touch access.log

36. Create a file named `README.txt` inside `devops`.  root@ip-172-31-28-15:~/devops# touch README.txt

37. Make a copy of `app.log` named `app_backup.log`.  root@ip-172-31-28-15:~/devops/logs# cp app.log app_backup.log

38. Copy `app.log` into the `backup` directory.   root@ip-172-31-28-15:~/devops# cp logs/app.log backup/app.log

39. Copy the complete `devops` directory into another test directory.  root@ip-172-31-28-15:~# cp -r devops test

40. Move `error.log` into the `backup` directory.  root@ip-172-31-28-15:~/devops# mv logs/error.log backup/error.log

41. Rename `access.log` to `web_access.log`. root@ip-172-31-28-15:~/devops/logs# mv access.log web_access.log

42. Rename the `scripts` directory to `automation`.  root@ip-172-31-28-15:~/devops# mv scripts automation

43. Remove a test file without affecting other files. test is not a file it is a directory

44. Remove an empty test directory.  rm test
45. Remove a test directory containing only disposable files. cannot find test with disposable files 

46. Create a new file by sending text from the shell into a file.  ??

47. Replace the entire contents of `app.log` with a single line of text. vi app.log ----my name is sahithi

48. Add another line to `app.log` while preserving the existing contents. vi app.log----my name is sahithi,i am completing my assesment

49. Add four separate lines to `app.log`. vi app.log----my name is sahithi
i am completing my assesment
i live in dudley
i completed my masters in data analytics 

50. Display all contents of `app.log`.  cat app.log---my name is sahithi
i am completing my assesment
i live in dudley
i completed my masters in data analytics 

51. Display all contents of `app.log` together with line numbers. cat -n app.log
     1  my name is sahithi
     2  i am completing my assesment
     3  i live in dudley
     4  i completed my masters in data analytics 

52. Display only the first three lines of `app.log`. cat -n app.log | head -n 3
     1  my name is sahithi
     2  i am completing my assesment
     3  i live in dudley

54. Display only the last three lines of `app.log`.  cat -n app.log | tail -n 3
     2  i am completing my assesment
     3  i live in dudley
     4  i completed my masters in data analytics 

55. Read a large text file interactively without loading it all at once.  cat app.log | more

56. Read a text file using a simple page-at-a-time viewer. no idea

57. Display the number of lines, words, and bytes in `app.log`. wc app.log
  4  20 107 app.log

58. Display only the number of lines in `app.log`. wc -l app.log
4 app.log

59. Search `app.log` for entries containing the word `ERROR`. r cat app.log | grep ERROR

60. Search a log for `error` regardless of letter case. cat app.log | grep -i error

61. Search all files under `devops` recursively for the word `ERROR`. no idea

62. Find every file ending in `.log` below the current directory.  find . -type f -name "*.log"
./web_access.log
./app_backup.log
./app.log

63. Find files modified during the last 24 hours.  no idea

64. Find files larger than 10 MB in a disposable test directory.

65. Find empty files under a test directory.

66. Compare two configuration files and identify their differences. diff "source" "destination"

67. Remove all contents from `app.log` while keeping the file itself. > app.log

68. Verify that `app.log` still exists after its contents were cleared. root@ip-172-31-28-15:~/devops/logs# ls app.log  app_backup.log  backup  we_baccess.log

69. Create `server.conf` and determine what kind of file it is. root@ip-172-31-28-15:~/devops# file server.conf

70. Display detailed filesystem metadata for `app.log`. stat app.log
  File: app.log
  size: 0               Blocks: 0          IO Block: 4096   regular empty file
Device: 259,1   Inode: 1829        Links: 1
Access: (0644/-rw-r--r--)  Uid: (    0/    root)   Gid: (    0/    root)
Access: 2026-09-06 17:33:40.600383719 +0000
Modify: 2026-09-06 17:33:35.939385124 +0000
Change: 2026-09-06 17:33:35.939385124 +0000
 Birth: 2026-09-06 17:19:50.350568702 +0000

71. Rename a file after verifying its current name and location. find /. type f -name file name, mv source destination

## 3. VI, REDIRECTION & TEXT PRACTICE

71. Open `app.log` in a terminal text editor.  cat app.log

72. Add a new line to `app.log` and save the file.   vi app.log---" i"---esc---:wq

73. Open a file, make a temporary change, and exit without saving.   vi app.log---"i"---esc--- :q!

74. Create `server.conf` using a terminal text editor. 

75. Verify the contents of a file after editing it. cat filename

76. Create a file containing the current date. no idea

77. Append the current uptime to an existing report without replacing its contents. no idea 

78. Create a five-line server report from shell-generated text.

79. Capture the output of a directory listing into `output.txt`.

80. Append another command's output to `output.txt`.

81. Create a log containing both normal output and error output from a test command.

82. Extract only failed/error entries from a log.

83. Display every line that does not contain `ERROR`.

84. Display the beginning and end of a large log for quick inspection.

85. Count the number of records in a text file. cat -n filename

86. Compare an original configuration with a modified copy. diff source1 source2

87. Check when a file was last modified and last accessed.

88. Determine whether a file is text, binary, or another recognized type. file filename

89. Find the executable location of three common Linux commands.

90. Read the documentation for a command and identify how to obtain its short usage/help information.

## 4. USER & GROUP MANAGEMENT

91. Create a user named `devuser` with a home directory. adduser devuser

92. Create a second test user named `deployuser`.  root@ip-172-31-28-15:~/home# adduser deployuser

93. Create a group named `devops`.  addgroup devops

94. Create a group named `developers`. addgroup developers

95. Set an initial password for `devuser`. 

96. Set an initial password for `deployuser`.  

97. Display the numeric user ID, primary group, and supplementary groups for `devuser`.  id devuser
uid=1004(devuser) gid=1004(devuser) groups=1004(devuser),100(users)

98. Display all groups to which `devuser` currently belongs.  groups devuser
devuser : devuser users

99. Add `devuser` to the `devops` supplementary group without removing existing supplementary groups.  usermod -aG devops devuser

100. Add `devuser` to the `developers` supplementary group while preserving previous memberships.   usermod -aG developers devuser

101. Verify the supplementary group memberships after the changes.  devuser@ip-172-31-28-15:~$ groups
devuser users devops developers

102. Force `devuser` to change the password at the next login. 

103. Lock the `devuser` account. usermod -L devuser

104. Verify that the account has been locked. root@ip-172-31-28-15:~# passwd -S devuser
devuser L 2026-09-06 0 99999 7 -1

105. Unlock the `devuser` account.  usermod -U devuser

106. Change the login shell of a test user.  no idea

107. Change the home directory of a disposable test user. no idea

108. Rename the `developers` group to `engineering`. root@ip-172-31-28-15:~# sudo groupmod -n engineering developers

109. Display the local user-account database.

110. Display the local group database.

111. Inspect the protected password/account database using appropriate privileges.

112. Count the number of local user entries. cat /etc/passwd | wc
     39      57    2061

113. Count the number of local group entries. 

114. Find the `devuser` entry in the local user database.  root@ip-172-31-28-15:~# cat /etc/passwd | grep -i devuser
devuser:x:1004:1004:,,,:/home/devuser:/bin/bash

115. Find the `devops` or renamed group entry in the local group database.  root@ip-172-31-28-15:~# cat /etc/group | grep -i devops
devops:x:1006:devuser

116. Display recent successful and unsuccessful login records available through the local login history.

117. If the user-information utility is installed, display information about `devuser`.

118. Delete a disposable test user and verify that the account no longer exists. sudo userdel test and cat /etc/passwd

119. Delete a disposable test group after ensuring no required users depend on it.  sudo groupdel test_group

120. Determine whether a test account is locked, expired, or otherwise restricted. sudo -S passwd

## 5. PERMISSIONS, OWNERSHIP & ACL

121. Display the permission bits, owner, and group of `app.log`. root@ip-172-31-28-15:~# ls -la | grep -i app.log
-rw-r--r--  1 root root        0 Sep  5 19:06 app.log

122. Set `app.log` so the owner can read/write, the group can read, and others can read. chmod 544 app.log

123. Set `deploy.sh` so the owner can read/write/execute and group/others can read/execute.  chmod 755 deploy.sh
root@ip-172-31-28-15:~# ls -la | grep -i deploy.sh
-rwxr-xr-x  1 root root        0 Sep  6 21:21 deploy.sh

124. Give only the owner execute permission on a test script.   chmod 100 test.sh
root@ip-172-31-28-15:~# ls -la | grep -i test.sh
---x------  1 root root        0 Sep  6 21:26 test.sh

125. Remove write permission for other users from a test file. chmod 775 test.sh
root@ip-172-31-28-15:~# ls -la | grep -i test.sh
-rwxrwxr-x  1 root root        0 Sep  6 21:26 test.sh

126. Give the group read and write access to a test file. chmod 060 test.sh

127. Remove group write access from a test file.chmod 050 test.sh

128. Set a test file so only its owner can read and write it. chmod 600 test.sh

129. Set a test file so the owner has full access and the group has read access. chmod 740 test.sh

130. Set a test directory so the owner has full access and the group can read/traverse it. chmod 740 test

131. Interpret the owner, group, and other permission fields shown for a file. ls- la | grep -i filename

132. Display numeric permission information and metadata for a file. 

133. Change the owner of a test file to `devuser`. chown devuser:root test.sh

134. Change the group of a test file to `devops`. chown root:devops test.sh

135. Change both the owner and group of a test file. chwon devuser:devops test.sh

136. Recursively correct ownership for a controlled project directory. 

137. Display the current default permission mask used when new files are created.

138. Temporarily change the default permission mask and observe permissions of a newly created file.

139. Temporarily change the default permission mask and observe permissions of a newly created directory.

140. Trace every directory component in a path and identify where traversal permission is missing.

141. Display ACL entries for a test file.

142. Give a test user additional read access to a file without changing the normal mode bits.

143. Verify the additional ACL permission.

144. Remove the test ACL entry and verify normal permissions.

145. Diagnose why a user cannot read a file by checking identity, ownership, mode bits, and ACLs.

146. Diagnose why a user cannot enter a directory by checking traversal permissions on every parent directory.

147. Diagnose why a script cannot execute even though the file exists.

148. Determine whether a particular user can write to a test directory.

149. Find world-writable files inside a controlled lab directory.

150. Find files owned by a specified user.

## 6. PROCESS MANAGEMENT

151. Display the processes associated with your current terminal.

152. Display every running process with its user and command information.

153. Display process IDs, users, CPU usage, and memory usage in a custom view.

154. Find a running process by name.

155. Find the process ID of the SSH server.

156. Find the process ID of nginx if it is installed and running.

157. Open an interactive process monitor.

158. Identify the process currently consuming the most CPU.

159. Identify the process currently consuming the most memory.

160. Produce a list of processes ordered from highest to lowest CPU usage.

161. Produce a list of processes ordered from highest to lowest memory usage.

162. Find the parent process ID of a selected process.

163. Display the parent-child process hierarchy.

164. Inspect the virtual process directory belonging to a selected PID.

165. Inspect the command line of a selected process through the process information filesystem.

166. Inspect the status information of a selected process through the process information filesystem.

167. Identify which files are currently open by a selected process.

168. Identify which process currently has a specified test file open.

169. Identify processes associated with network sockets.

170. Start a controlled sleep process and identify its PID.

171. Gracefully terminate the controlled process.

172. Force-terminate a disposable test process that does not respond to normal termination.

173. Verify that a terminated process is no longer running.

174. Create a controlled high-CPU workload on a disposable server.

175. Identify the high-CPU workload and record its PID.

176. Stop the controlled high-CPU workload safely.

177. Display the scheduling priority and nice value of a selected process.

178. Start a disposable process with a changed scheduling priority.

179. Find the start time of a selected process.

180. Investigate a process that appears to be hung or unresponsive.

## 7. BACKGROUND JOBS & JOB CONTROL

181. Start a long-running sleep command as a background job.

182. Display the background jobs belonging to the current shell.

183. Display the process ID associated with a background job.

184. Bring a background job into the foreground.

185. Pause a foreground test job and return it to the background.

186. Resume a stopped background job.

187. Start two background jobs and identify each job number.

188. Match a shell job number to its process ID.

189. Terminate a background test job.

190. Verify that the background job has ended.

191. Run a long command in the background while writing its output to a log file.

192. Display background jobs together with their process IDs.

193. Find a background process using the normal process list.

194. Find a background process by name.

195. Practice moving a disposable sleep process between foreground and background states.

## 8. PERFORMANCE MONITORING

196. Display current virtual-memory, process, CPU, and I/O statistics.

197. Collect five performance samples at two-second intervals.

198. Use virtual-memory statistics to determine whether processes are waiting for CPU time.

199. Use virtual-memory statistics to inspect memory and swap activity.

200. Use virtual-memory statistics to inspect I/O wait activity.

201. Use performance statistics to investigate a simulated slow server.

202. Determine whether swap is currently being used.

203. Display detailed memory pressure information.

204. If system activity reporting is installed, display current CPU statistics.

205. Collect repeated CPU samples using the system activity reporter.

206. Use the system activity reporter to inspect memory statistics.

207. Use the system activity reporter to inspect network-interface statistics.

208. Determine whether CPU, memory, or I/O is the primary bottleneck from collected evidence.

209. Compare process-monitor, virtual-memory, and activity-reporting results.

210. Write a short evidence-based diagnosis for a simulated performance incident.

## 9. SYSTEM MANAGEMENT & SERVICES

211. List all currently running services managed by the system service manager.

212. List all loaded service units.

213. List services that are currently in a failed state.

214. Check the current state of a selected service.

215. Start a stopped test service.

216. Stop a running test service.

217. Restart a test service.

218. Reload a service configuration without fully stopping the service where supported.

219. Configure a service to start automatically during boot.

220. Determine whether a service is enabled for boot.

221. Disable a disposable test service from automatic startup.

222. Find the unit-file location of a service.

223. Display the dependencies of a selected service.

224. Identify the processes belonging to a service.

225. Identify the network port used by a service.

226. Display recent journal entries belonging to a service.

227. Follow service logs while reproducing a test failure.

228. Display the most recent 100 entries for a service.

229. Identify all failed service units.

230. Determine why a service failed to start.

231. Correlate service status, process state, listening ports, and journal entries.

232. Verify a service after restarting it.

233. Identify services configured to start automatically at boot.

234. Display logs from the current system boot.

235. Display recent kernel messages and identify warnings or errors.

## 10. PACKAGE MANAGEMENT

236. Refresh the local package index.

237. Search the package repositories for a package that provides a common utility.

238. Display detailed information about a package before installing it.

239. Display package information using the package-cache database.

240. Determine the installed version and repository candidate version of a package.

241. Install a small test package.

242. Verify that the package is installed.

243. Find an installed package by searching the installed-package database.

244. Display the detailed installation status of an installed package.

245. List files installed by a selected package.

246. Determine which installed package owns a particular file where supported.

247. Upgrade one installed package without upgrading unrelated packages.

248. Upgrade available packages on a disposable lab server.

249. Review the output of a package upgrade and identify changed packages.

250. Remove a disposable test package while keeping configuration files where applicable.

251. Completely purge a disposable test package and its configuration files where appropriate.

252. Remove unused dependencies that are no longer required.

253. Remove downloaded package archives from the local cache.

254. Review package installation, upgrade, and removal history.

255. Inspect the package database log for recent transactions.

256. Inspect the package-manager history log for recent transactions.

257. Diagnose a failed package installation using repository and package-manager evidence.

258. Diagnose a broken dependency situation in a disposable test environment.

259. Verify package state after completing an upgrade.

260. Determine whether a command is available after installing its expected package.

## 11. CRONTAB & SCHEDULED JOBS

261. Display the current user's scheduled cron entries.

262. Open the current user's cron schedule for editing.

263. Create a scheduled job that writes the current date to `/tmp/cron_test.log` every minute.

264. Verify that the new scheduled job is present.

265. Wait for the scheduled job to execute and verify its output.

266. Create a scheduled job that appends server uptime to a log every minute.

267. Capture both normal output and error output from a scheduled job into a log.

268. Create a script named `monitor_server.sh` for scheduled monitoring.

269. Give `monitor_server.sh` the permissions required to execute.

270. Schedule `monitor_server.sh` to run at a defined interval.

271. Check whether the cron service is running.

272. Inspect scheduled-job execution records in the system journal where supported.

273. Inspect system log entries for cron execution on systems using syslog.

274. Create a scheduled job that preserves previous log entries rather than replacing the file.

275. Remove a test scheduled job and verify that it is gone.

## 12. NETWORKING & CONNECTIVITY

276. Display all network interfaces and their assigned addresses.

277. Display the routing table.

278. Identify the default gateway.

279. Identify the interface used for the default route.

280. Display network-interface statistics.

281. Test basic reachability to another host.

282. Resolve a hostname and inspect the DNS response.

283. Query the IPv4 address record for a hostname.

284. Query the mail-exchange records for a domain.

285. Resolve a hostname using an alternate DNS lookup utility.

286. Inspect the resolver configuration used by the server.

287. Test an HTTP endpoint and inspect the response.

288. Display only the HTTP response headers from a web server.

289. Use verbose HTTP diagnostics to determine where a request is failing.

290. Display all listening TCP and UDP sockets together with owning processes.

291. Display listening TCP sockets and their owning processes.

292. Identify the process listening on port 22.

293. Identify the process listening on port 80.

294. Identify the process listening on port 443.

295. Identify the process listening on port 8080.

296. Identify which process owns a specified TCP port.

297. Identify which process owns a second specified TCP port.

298. Test whether a remote TCP port can be reached.

299. Test reachability of the SSH port on a test server.

300. Test reachability of the HTTP port on a test server.

## PRACTICE WORKFLOW

Read the mission → Decide what evidence is needed → Discover the command → Execute safely → Verify → Document

## SAFETY

Use a disposable/test Linux server for disruptive exercises. Be especially careful with recursive deletion, account deletion, package removal, service changes, process termination, firewall changes, and disk-pressure tests.
