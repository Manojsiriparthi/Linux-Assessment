# Linux-Assessment
This repo contains TASKS ONLY. No command names, command options, or solutions are intentionally given as hints. Use your Linux knowledge, manual pages, built-in help, and lab experimentation to discover the commands.

# LINUX DEVOPS PRACTICAL PRACTICE — 300 TASKS

## TASK-ONLY WORKBOOK

This file contains TASKS ONLY.
No command names, command options, or solutions are intentionally given as hints.
Use your Linux knowledge, manual pages, built-in help, and lab experimentation to discover the commands.

For every mission, record separately: command discovered, important output, diagnosis, action, and verification.

## 1. FILESYSTEM HIERARCHY & LINUX BASICS

1. Find the username of the account currently running your shell.
root@ip-10-0-1-140:~# whoami
root
root@ip-10-0-1-140:~# id
uid=0(root) gid=0(root) groups=0(root)
root@ip-10-0-1-140:~# 
root@ip-10-0-1-140:~# 


2. Find the absolute path of your current working directory.

3. Find the Linux kernel release currently running on the server.

4. Find the Linux system/kernel name.

5. Display complete kernel and system information.

6. Identify the Linux distribution and release version.

7. Find the server's configured hostname.

8. Identify whether the server is 32-bit or 64-bit.

9. Display the current date and time.

10. Find how long the server has been running and its current load averages.

11. Identify the CPU model used by the server.

12. Find the number of logical CPUs available.

13. Display total, used, free, and available memory.

14. Display disk space usage for all mounted filesystems in a human-readable format.

15. Explore the system configuration directory and identify at least five important configuration files.

16. Explore the system log directory and identify the major system/service logs present.

17. Identify the home directories belonging to normal users.

18. Find the home directory used by the superuser account.

19. Inspect the temporary-file directory and identify its purpose.

20. Identify where common user-space programs and libraries are stored.

21. Identify the standard location used for optional third-party applications.

22. Explore device files and identify examples representing disks or terminals.

23. Explore the process-information virtual filesystem and identify directories belonging to running processes.

24. Explore the kernel/device virtual filesystem and identify information about devices.

25. Explore runtime state files and identify examples of PID files or sockets.

26. Locate the server-side remote-login configuration directory.

27. Locate the current user's remote-login configuration and key directory.

28. Find the executable path of a common command available on the server.

29. Read the built-in documentation for a common Linux command and identify five useful options.

30. Create a short system-information report containing the hostname, kernel, uptime, CPU, memory, and disk information.

## 2. FILE & DIRECTORY MANAGEMENT

31. Create a file named `app.log`.

32. Create a directory named `devops`.

33. Create the nested directory structure `devops/project/src` in one operation.

34. Create `logs`, `scripts`, and `backup` inside the `devops` directory.

35. Create `app.log`, `error.log`, and `access.log` inside `devops/logs`.

36. Create a file named `README.txt` inside `devops`.

37. Make a copy of `app.log` named `app_backup.log`.

38. Copy `app.log` into the `backup` directory.

39. Copy the complete `devops` directory into another test directory.

40. Move `error.log` into the `backup` directory.

41. Rename `access.log` to `web_access.log`.

42. Rename the `scripts` directory to `automation`.

43. Remove a test file without affecting other files.

44. Remove an empty test directory.

45. Remove a test directory containing only disposable files.

46. Create a new file by sending text from the shell into a file.

47. Replace the entire contents of `app.log` with a single line of text.

48. Add another line to `app.log` while preserving the existing contents.

49. Add four separate lines to `app.log`.

50. Display all contents of `app.log`.

51. Display all contents of `app.log` together with line numbers.

52. Display only the first three lines of `app.log`.

53. Display only the last three lines of `app.log`.

54. Read a large text file interactively without loading it all at once.

55. Read a text file using a simple page-at-a-time viewer.

56. Display the number of lines, words, and bytes in `app.log`.

57. Display only the number of lines in `app.log`.

58. Search `app.log` for entries containing the word `ERROR`.

59. Search a log for `error` regardless of letter case.

60. Search all files under `devops` recursively for the word `ERROR`.

61. Find every file ending in `.log` below the current directory.

62. Find files modified during the last 24 hours.

63. Find files larger than 10 MB in a disposable test directory.

64. Find empty files under a test directory.

65. Compare two configuration files and identify their differences.

66. Remove all contents from `app.log` while keeping the file itself.

67. Verify that `app.log` still exists after its contents were cleared.

68. Create `server.conf` and determine what kind of file it is.

69. Display detailed filesystem metadata for `app.log`.

70. Rename a file after verifying its current name and location.

## 3. VI, REDIRECTION & TEXT PRACTICE

71. Open `app.log` in a terminal text editor.

72. Add a new line to `app.log` and save the file.

73. Open a file, make a temporary change, and exit without saving.

74. Create `server.conf` using a terminal text editor.

75. Verify the contents of a file after editing it.

76. Create a file containing the current date.

77. Append the current uptime to an existing report without replacing its contents.

78. Create a five-line server report from shell-generated text.

79. Capture the output of a directory listing into `output.txt`.

80. Append another command's output to `output.txt`.

81. Create a log containing both normal output and error output from a test command.

82. Extract only failed/error entries from a log.

83. Display every line that does not contain `ERROR`.

84. Display the beginning and end of a large log for quick inspection.

85. Count the number of records in a text file.

86. Compare an original configuration with a modified copy.

87. Check when a file was last modified and last accessed.

88. Determine whether a file is text, binary, or another recognized type.

89. Find the executable location of three common Linux commands.

90. Read the documentation for a command and identify how to obtain its short usage/help information.

## 4. USER & GROUP MANAGEMENT

91. Create a user named `devuser` with a home directory.

92. Create a second test user named `deployuser`.

93. Create a group named `devops`.

94. Create a group named `developers`.

95. Set an initial password for `devuser`.

96. Set an initial password for `deployuser`.

97. Display the numeric user ID, primary group, and supplementary groups for `devuser`.

98. Display all groups to which `devuser` currently belongs.

99. Add `devuser` to the `devops` supplementary group without removing existing supplementary groups.

100. Add `devuser` to the `developers` supplementary group while preserving previous memberships.

101. Verify the supplementary group memberships after the changes.

102. Force `devuser` to change the password at the next login.

103. Lock the `devuser` account.

104. Verify that the account has been locked.

105. Unlock the `devuser` account.

106. Change the login shell of a test user.

107. Change the home directory of a disposable test user.

108. Rename the `developers` group to `engineering`.

109. Display the local user-account database.

110. Display the local group database.

111. Inspect the protected password/account database using appropriate privileges.

112. Count the number of local user entries.

113. Count the number of local group entries.

114. Find the `devuser` entry in the local user database.

115. Find the `devops` or renamed group entry in the local group database.

116. Display recent successful and unsuccessful login records available through the local login history.

117. If the user-information utility is installed, display information about `devuser`.

118. Delete a disposable test user and verify that the account no longer exists.

119. Delete a disposable test group after ensuring no required users depend on it.

120. Determine whether a test account is locked, expired, or otherwise restricted.

## 5. PERMISSIONS, OWNERSHIP & ACL

121. Display the permission bits, owner, and group of `app.log`.

122. Set `app.log` so the owner can read/write, the group can read, and others can read.

123. Set `deploy.sh` so the owner can read/write/execute and group/others can read/execute.

124. Give only the owner execute permission on a test script.

125. Remove write permission for other users from a test file.

126. Give the group read and write access to a test file.

127. Remove group write access from a test file.

128. Set a test file so only its owner can read and write it.

129. Set a test file so the owner has full access and the group has read access.

130. Set a test directory so the owner has full access and the group can read/traverse it.

131. Interpret the owner, group, and other permission fields shown for a file.

132. Display numeric permission information and metadata for a file.

133. Change the owner of a test file to `devuser`.

134. Change the group of a test file to `devops`.

135. Change both the owner and group of a test file.

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
