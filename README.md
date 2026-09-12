# Linux-Assessment
This repo contains TASKS ONLY. No command names, command options, or solutions are intentionally given as hints. Use your Linux knowledge, manual pages, built-in help, and lab experimentation to discover the commands.

# LINUX DEVOPS PRACTICAL PRACTICE — 300 TASKS

## TASK-ONLY WORKBOOK

This file contains TASKS ONLY.
No command names, command options, or solutions are intentionally given as hints.
Use your Linux knowledge, manual pages, built-in help, and lab experimentation to discover the commands.

For every mission, record separately: command discovered, important output, diagnosis, action, and verification.

## 1. FILESYSTEM HIERARCHY & LINUX BASICS

1. Find the username of the account currently running your shell.------- whoami <img width="730" height="176" alt="image" src="https://github.com/user-attachments/assets/3f62c52f-3955-45bb-a9fe-de69ed682837" />


2. Find the absolute path of your current working directory.--------- pwd <img width="856" height="224" alt="image" src="https://github.com/user-attachments/assets/4f046f7c-21ed-4976-afa2-df040c8a5125" />


3. Find the Linux kernel release currently running on the server.------- uname -r <img width="848" height="372" alt="image" src="https://github.com/user-attachments/assets/90b78d33-8d55-4515-90a9-c884574dfdf7" />


4. Find the Linux system/kernel name.--------- uname -s  <img width="810" height="334" alt="image" src="https://github.com/user-attachments/assets/6ab0ad43-0310-4d67-94b2-4f21e48f5c6a" />


5. Display complete kernel and system information.--------- uname -a <img width="2416" height="384" alt="image" src="https://github.com/user-attachments/assets/5dbc936c-f27b-4faf-8327-4e9a3c35cf3c" />


6. Identify the Linux distribution and release version. ------ cat /etc/os-release <img width="2336" height="1032" alt="image" src="https://github.com/user-attachments/assets/57ef3e1f-639b-4b44-8e13-8152e458da1b" />


7. Find the server's configured hostname.------------- hostname  <img width="1192" height="314" alt="image" src="https://github.com/user-attachments/assets/2fcd3235-de25-4482-ae6b-de17a11c2428" />


8. Identify whether the server is 32-bit or 64-bit. ---------- uname -m <img width="952" height="334" alt="image" src="https://github.com/user-attachments/assets/20f669c6-3a81-4a5a-bbb7-5fdcd3c81d73" />


9. Display the current date and time. ---------- date <img width="886" height="292" alt="image" src="https://github.com/user-attachments/assets/75bbb9cb-161c-4c73-b96e-31b4981d775a" />


10. Find how long the server has been running and its current load averages. ------- uptime <img width="1740" height="432" alt="image" src="https://github.com/user-attachments/assets/b21d8344-609e-4a81-a72a-4b75f282699c" />


11. Identify the CPU model used by the server.---------  lscpu | grep -i "model name" <img width="2412" height="292" alt="image" src="https://github.com/user-attachments/assets/e6b53299-108a-4896-b2f2-0ead5094ec0b" />

12. Find the number of logical CPUs available. ------- lscpu <img width="2174" height="372" alt="image" src="https://github.com/user-attachments/assets/5eff7f10-a38f-41d0-9e89-a998cc454f2c" />


13. Display total, used, free, and available memory.-------- free -h <img width="2322" height="440" alt="image" src="https://github.com/user-attachments/assets/ba22f593-dc7e-4288-ab3a-cdf1be505572" />


14. Display disk space usage for all mounted filesystems in a human-readable format. ------- df -h <img width="2290" height="882" alt="image" src="https://github.com/user-attachments/assets/e00fc91a-8422-416f-af94-74089e5e5f84" />


15. Explore the system configuration directory and identify at least five important configuration files. -------ls -l/etc <img width="1782" height="1348" alt="image" src="https://github.com/user-attachments/assets/2a3f45f9-b472-4405-b7ad-8f8be0b0c1dc" />


16. Explore the system log directory and identify the major system/service logs present.--------- sudo ls -lh/var/log <img width="2216" height="1394" alt="image" src="https://github.com/user-attachments/assets/8fe20058-7a30-4cd4-8817-ac9537ffd1be" />


17. Identify the home directories belonging to normal users.-------- ls -la /home <img width="1324" height="298" alt="image" src="https://github.com/user-attachments/assets/0f90b7a9-0d76-4faa-ade9-45ebdd397bfc" />


18. Find the home directory used by the superuser account.

19. Inspect the temporary-file directory and identify its purpose.---------  ls -ld /tmp <img width="1186" height="300" alt="image" src="https://github.com/user-attachments/assets/7e52a109-b276-4e20-9339-29dc1d9f086f" />


20. Identify where common user-space programs and libraries are stored.----- ls -ld /lib* <img width="1306" height="296" alt="image" src="https://github.com/user-attachments/assets/6499ab0f-1fc0-46bc-8824-76055d3fb3b2" />



21. Identify the standard location used for optional third-party applications. -------- ls -la /opt <img width="1418" height="244" alt="image" src="https://github.com/user-attachments/assets/fd06da17-f776-4151-a762-829f17938e43" />


22. Explore device files and identify examples representing disks or terminals.--------  ls -l/dev <img width="2042" height="1326" alt="image" src="https://github.com/user-attachments/assets/e7ca683a-f36d-4c73-be45-05c28cad4176" />


23. Explore the process-information virtual filesystem and identify directories belonging to running processes. ------- ps aux <img width="2756" height="1136" alt="image" src="https://github.com/user-attachments/assets/00f3c938-03bb-401d-918a-0694ad6af0fb" />


24. Explore the kernel/device virtual filesystem and identify information about devices. ------ ls -la /sys/class      <img width="1680" height="1168" alt="image" src="https://github.com/user-attachments/assets/4d052cff-3a08-4f32-829e-358b8b1b9da2" />


25. Explore runtime state files and identify examples of PID files or sockets. ------- ls -la /run<img width="1876" height="1128" alt="image" src="https://github.com/user-attachments/assets/903265ba-5f63-414b-aeaa-19433b6ca987" />


26. Locate the server-side remote-login configuration directory. 

27. Locate the current user's remote-login configuration and key directory.------ sudo systemctl status ssh <img width="2392" height="1160" alt="image" src="https://github.com/user-attachments/assets/33ade468-1fee-4d1f-9e2e-263b3e737433" />


28. Find the executable path of a common command available on the server.------ which ls <img width="1260" height="346" alt="image" src="https://github.com/user-attachments/assets/a80c6e7e-0ce0-46af-91e0-d63d27ab2b17" />


29. Read the built-in documentation for a common Linux command and identify five useful options.  ------- man ls <img width="2902" height="1154" alt="image" src="https://github.com/user-attachments/assets/b1cb40a1-32d4-4d26-b153-8bdb12c473f8" />


30. Create a short system-information report containing the hostname, kernel, uptime, CPU, memory, and disk information. --  top,htop,glance <img width="2514" height="1176" alt="image" src="https://github.com/user-attachments/assets/e7bf5b2b-5509-47fb-84b7-407f0aba8e5c" />


## 2. FILE & DIRECTORY MANAGEMENT

31. Create a file named `app.log`. ----- touch app.log <img width="1094" height="344" alt="image" src="https://github.com/user-attachments/assets/7e130de5-2a10-444f-a27d-8f5e66416442" />


32. Create a directory named `devops`. ------- mkdir devops <img width="1390" height="340" alt="image" src="https://github.com/user-attachments/assets/b471212d-cdb0-45a8-acaf-f69be3d51b9b" />


33. Create the nested directory structure `devops/project/src` in one operation. ------ mkdir -p devops/project/src   <img width="1790" height="718" alt="image" src="https://github.com/user-attachments/assets/77cd2b18-6fc3-4b4b-bffc-b03a9d97914c" />


34. Create `logs`, `scripts`, and `backup` inside the `devops` directory. ------- mkdir -p devops/{logs,scripts,backup}
    <img width="2106" height="784" alt="image" src="https://github.com/user-attachments/assets/2b96e36a-d569-4b5a-a48b-447b37dd661e" />


36. Create `app.log`, `error.log`, and `access.log` inside `devops/logs`. -------- touch app.log error.log access.log
    <img width="1626" height="298" alt="image" src="https://github.com/user-attachments/assets/4ffe2800-7690-4b09-9ba7-59e1ef0e552d" />

37. Make a copy of app.log named app_backup.log. --------  cp app.log app_backup.log <img width="1884" height="546" alt="image" src="https://github.com/user-attachments/assets/d2c8cffb-9075-45d5-90a4-680ce497c3f0" />


38. Create a file named `README.txt` inside `devops`. -----------  touch devops/README.txt   <img width="1592" height="528" alt="image" src="https://github.com/user-attachments/assets/6b7ea597-c9b8-4e13-8a92-7f55e12b1a6e" />
    

39. Make a copy of `app.log` named `app_backup.log`. --------- cp devops/logs/app.log devops/logs/app_backup.log     <img width="2504" height="526" alt="image" src="https://github.com/user-attachments/assets/ecb3889d-23e7-4450-9a7b-ca98ea685213" />

40. Copy `app.log` into the `backup` directory. --------- cp app.log devops/backup/    <img width="2058" height="1096" alt="image" src="https://github.com/user-attachments/assets/19bbd76b-aa90-4f54-8b36-f4ec5b1738f8" />


41. Copy the complete `devops` directory into another test directory.---- cp -r devops test.    <img width="1564" height="382" alt="image" src="https://github.com/user-attachments/assets/90a443c8-8b92-4ad6-8d66-23b8622b0a0a" />


42. Move `error.log` into the `backup` directory. --------- mv devops/logs/error.log devops/backup/    <img width="2154" height="320" alt="image" src="https://github.com/user-attachments/assets/56c90ed6-f87b-4719-9784-89c2b48d0fec" />

43. Rename `access.log` to `web_access.log`.-------- mv devops/logs/access.log devops/logs/web_access.log <img width="2602" height="354" alt="image" src="https://github.com/user-attachments/assets/e437b462-1311-4b9a-adbd-14db4af615cd" />


44. Rename the `scripts` directory to `automation`.-------- mv devops/scripts devops/automation <img width="2090" height="328" alt="image" src="https://github.com/user-attachments/assets/df196c10-7868-4b51-b3e7-b4443cc6146f" />


45. Remove a test file without affecting other files.----- rm test file.  <img width="1600" height="870" alt="image" src="https://github.com/user-attachments/assets/cd515258-3ea9-49eb-8f0a-4473598f50fa" />


46. Remove an empty test directory. ------ rmdir testdirectory.  <img width="1822" height="710" alt="image" src="https://github.com/user-attachments/assets/1d35bf8c-53cb-41f7-9ffd-2931c2b685e0" />


47. Remove a test directory containing only disposable files.------- rm -r disposable <img width="2382" height="728" alt="image" src="https://github.com/user-attachments/assets/7ce2d7e9-2f99-4a57-bd21-57c29c8ecfcc" />


48. Create a new file by sending text from the shell into a file. -------- echo "Hello people, welcome to the class" > newfile.txt   <img width="1800" height="390" alt="image" src="https://github.com/user-attachments/assets/0298c3aa-0d49-41b9-b8bd-781a4821c1d9" />


49. Replace the entire contents of `app.log` with a single line of text. ------ echo "This is my first commit." > app.log  <img width="2116" height="1078" alt="image" src="https://github.com/user-attachments/assets/37b0304f-772f-451d-afed-44d2515262aa" />


50. Add another line to `app.log` while preserving the existing contents. - echo "this is my second commit." >>app.log <img width="1548" height="300" alt="image" src="https://github.com/user-attachments/assets/d6f0c617-e540-4d48-93b0-00975b01cf00" />


51. Add four separate lines to `app.log`. ---- vi app.log <img width="978" height="464" alt="image" src="https://github.com/user-attachments/assets/f01ae267-eb63-4e47-85f0-21b4e1d128ea" />


52. Display all contents of `app.log`. <img width="978" height="464" alt="image" src="https://github.com/user-attachments/assets/aeaa5833-1a8f-4ecb-9b00-8e92ce15650c" />


53. Display all contents of `app.log` together with line numbers. cat -n app.log <img width="926" height="348" alt="image" src="https://github.com/user-attachments/assets/6403146c-4bf4-4c49-a2c2-ca9a23407d58" />


54. Display only the first three lines of `app.log`. -------  head -n 3 app.log <img width="1268" height="338" alt="image" src="https://github.com/user-attachments/assets/5a28d66f-04bf-457b-8fa4-862023d4d649" />

55. Display only the last three lines of `app.log' ------   tail -n 3 app.log <img width="1040" height="270" alt="image" src="https://github.com/user-attachments/assets/bb054582-2001-4af3-bd63-5af626c9f821" />

    
57.   Read a large text file interactively without loading it all at once. less app.log <img width="2478" height="1472" alt="image" src="https://github.com/user-attachments/assets/126206d2-f276-4111-8751-030a0330e7ca" />

59. Read a text file using a simple page-at-a-time viewer. more app.log <img width="798" height="370" alt="image" src="https://github.com/user-attachments/assets/f45a01cc-44af-4b65-911c-7b7d6c7aa114" />


60. Display the number of lines, words, and bytes in `app.log`. wc app.log <img width="1006" height="240" alt="image" src="https://github.com/user-attachments/assets/607f5d82-391b-4a6c-a036-5ed99604d85a" />


61. Display only the number of lines in `app.log`.------ wc -l app.log <img width="948" height="238" alt="image" src="https://github.com/user-attachments/assets/a64948de-a3ab-4169-a9cc-0e86360992b1" />


62. Search `app.log` for entries containing the word `ERROR`. ----- grep "ERROR" app.log <img width="1394" height="176" alt="image" src="https://github.com/user-attachments/assets/28f5a2bc-3b81-4f34-8e89-446bb310d0fb" />


63. Search a log for `error` regardless of letter case. ------ grep -i "error" app.log <img width="1304" height="334" alt="image" src="https://github.com/user-attachments/assets/dbe6fadc-9a5b-40f7-9e65-f2057852c105" />


64. Search all files under `devops` recursively for the word `ERROR`. ------- grep -r "ERROR" devops/  <img width="1262" height="390" alt="image" src="https://github.com/user-attachments/assets/63fc5e7b-9b64-487b-8075-29170f80fccf" />


65. Find every file ending in `.log` below the current directory. find / -type f -name "*.log" <img width="1288" height="556" alt="image" src="https://github.com/user-attachments/assets/3d377b26-2226-4459-a111-3a5c9571caaa" />


66. Find files modified during the last 24 hours. find . -type f -mtime -1  <img width="1242" height="382" alt="image" src="https://github.com/user-attachments/assets/6c6bf852-7c85-4617-8f07-39223c40b290" />


67. Find files larger than 10 MB in a disposable test directory. find test -type f -size +10M <img width="1232" height="278" alt="image" src="https://github.com/user-attachments/assets/94625940-86e3-47a7-87e4-cf6c6aba2559" />


68. Find empty files under a test directory. find test -type f -empty <img width="1570" height="450" alt="image" src="https://github.com/user-attachments/assets/1bd81fb1-c457-40db-9ad1-b5aeee9e9d12" />

    
70. Compare two configuration files and identify their differences. diff config1.conf config2.conf. <img width="1354" height="370" alt="image" src="https://github.com/user-attachments/assets/939827da-16d0-4226-ac81-5c6b217bbf03" />


71. Remove all contents from `app.log` while keeping the file itself. > app.log <img width="1358" height="512" alt="image" src="https://github.com/user-attachments/assets/f4d31db3-a2cb-454b-bae0-eefdaf7a8fd5" />

72. Verify that `app.log` still exists after its contents were cleared. ------ ls -l app.log <img width="1132" height="366" alt="image" src="https://github.com/user-attachments/assets/63194f5f-70ce-4e74-9de7-292c41596066" />

. Create `server.conf` and determine what kind of file it is.

74. Display detailed filesystem metadata for `app.log`.

75. Rename a file after verifying its current name and location.

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
