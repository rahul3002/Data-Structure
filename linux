
## Linux

<details>
<summary>What is your experience with Linux?</summary><br><b>

Only you know :)

For example:
* Administration
* Troubleshooting & Debugging
* Storage
* Networking
* Development
* Deployments
</b></details>

<details>
<summary>Explain what each of the following commands does and give an example on how to use it:

  * touch
  * ls
  * rm
  * cat
  * cp
  * mkdir
</summary><br><b>
</b></details>

<details>
<summary>Some of the commands in the previous question can be run with the -r/--recursive flag. What does it do?</summary><br><b>
</b></details>

<details>
<summary>Explain each field in the output of `ls -l` command</summary><br><b>
It shows a detailed list of files in a long format. From the left:

* file permissions, number of links, owner name, owner group, file size, timestamp of last modification and directory/file name
</b></details>

<details>
<summary>What are hidden files/directories? How to list them?</summary><br><b>
These are files directly not displayed after performing a standard ls direct listing. An example of these files are .bashrc which are used to execute some scripts. Some also store configuration about services on your host like .KUBECONFIG. The command used to list them is,

`ls -a`
</b></details>

<details>
<summary>Explain what each of the following commands does and give an example on how to use it:

  * sed
  * grep
  * cut
  * awk
</summary><br><b>
</b></details>

<details>
<summary>What each of the following commands does?

  * pwd
  * cd
  * find
  * ls
</summary><br><b>
</b></details>

<details>
<summary>What each of the following commands does?

  * cd /
  * cd ~
  * cd
  * cd ..
  * cd .
  * cd -
</summary><br><b>

  * cd / -> change to the root directory
  * cd ~ -> change to your home directory
  * cd -> change to your home directory
  * cd .. -> change to the directory above your current i.e parent directory
  * cd . -> change to the directory you currently in
  * cd - -> change to the last visited path
</b></details>

<details>
<summary>How to rename the name of a file or a directory?</summary><br><b>

Using the `mv` command.
</b></details>

<details>
<summary>Specify which command would you use (and how) for each of the following scenarios 

  * Remove a directory with files
  * Display the content of a file
  * Provides access to the file /tmp/x for everyone
  * Change working directory to user home directory
  * Replace every occurrence of the word "good" with "great" in the file /tmp/y</summary><br><b>
</b></details>

<details>
<summary>How can you check what is the path of a certain command?</summary><br><b>

  * whereis
  * which
</b></details>

<details>
<summary>Explain redirection</summary><br><b>
</b></details>

<details>
<summary>Explain piping. How do you perform piping?</summary><br><b>

Using a pipe in Linux, allows you to send the output of one to another (also called redirection). For example: `cat /etc/services | wc -l`
</b></details>

<details>
<summary>Fix the following commands:

  * sed "s/1/2/g' /tmp/myFile
  * find . -iname \*.yaml -exec sed -i "s/1/2/g" {} ;

  </summary><br><b>
</b>
<code>sed 's/1/2/g' /tmp/myFile</code><br>
<code> find . -iname "*.yaml" -exec sed -i "s/1/2/g" {} \; </code>
</details>

#### Linux FHS

<details>
<summary>In Linux FHS (Filesystem Hierarchy Standard) what is the <code>/</code>?</summary><br><b>
</b></details>

<details>
<summary>What is stored in each of the following paths?

  * /bin, /sbin, /usr/bin and /usr/sbin
  * /etc
  * /home
  * /var
  * /tmp</summary><br><b>
</b></details>

<details>
<summary>What is special about the /tmp directory when compared to other directories?</summary><br><b>
</b></details>

<details>
<summary>What kind of information one can find in /proc?</summary><br><b>
</b></details>

<details>
<summary>Can you create files in /proc?</summary><br><b>
</b></details>

<details>
<summary>In which path can you find the system devices (e.g. block storage)?</summary><br><b>
</b></details>

<details>
<summary>Running the command <code>df</code> you get "command not found". What could be wrong and how to fix it?</summary><br><b>
</b>
<p><b>
Most likely the default/generated $PATH was somehow modified or overridden thus not containing <code>/bin/</code> where df would normally go.
This issue could also happen if bash_profile or any configuration file of your interpreter was wrongly modified, causing erratics behaviours.
You would solve this by fixing your $PATH variable:

As to fix it there are several options:

1. Manually adding what you need to your $PATH <code>PATH="$PATH":/user/bin:/..etc</code>
2. You have your weird env variables backed up.
3. You would look for your distro default $PATH variable, copy paste using method #1

Note: There are many ways of getting errors like this: if bash_profile or any configuration file of your interpreter was wrongly modified; causing erratics behaviours,
permissions issues, bad compiled software (if you compiled it by yourself)... there is no answer that will be true 100% of the time.
</b>
</p>
</details>

<details>
<summary>How do you schedule tasks periodically?</summary><br><b>

You can use the commands <code>cron</code> and <code>at</code>.
With cron, tasks are scheduled using the following format:

<code>*/30 * * * * bash myscript.sh</code> Executes the script every 30 minutes.

<minute> <hour> <day of month> <month> <day of week> <command to execute>

The tasks are stored in a cron file, you can write in it using <code>crontab -e</code>

Alternatively if you are using a distro with systemd it's recommended to use systemd timers.
</b></details>

<details>
<summary>How to check which commands you executed in the past?</summary><br><b>

history command or .bash_history file
</b></details>

##### Linux Permissions

<details>
<summary>How to change the permissions of a file?</summary><br><b>

Using the `chmod` command.
</b></details>

<details>
<summary>What does the following permissions mean?:

  * 777
  * 644
  * 750</summary><br><b>

<pre>
777 - You give the owner, group and other: Execute (1), Write (2) and Read (4); 4+2+1 = 7.
644 - Owner has Read (4), Write (2), 4+2 = 6; Group and Other have Read (4).
750 - Owner has x+r+w, Group has Read (4) and Execute (1); 4+1 = 5. Other have no permissions.
</pre>
</b></details>

<details>
<summary>What this command does? <code>chmod +x some_file</code></summary><br><b>
It adds execute permissions to all sets i.e user, group and others
</b></details>

<details>
<summary>Explain what is setgid and setuid</summary><br><b>

* setuid is a linux file permission that permits a user to run a file or program with the permissions of the owner of that file. This is possible by elevation of current user privileges.
* setgid is a process when executed will run as the group that owns the file.
</b></details>

<details>
<summary>What is the purpose of sticky bit?</summary><br><b>
Its a bit that only allows the owner or the root user to delete or modify the file.
</b></details>

<details>
<summary>What the following commands do?

  * chmod
  * chown
  * chgrp</summary><br><b>

  * chmod - changes access permissions to files system objects
  * chown - changes the owner of file system files and directories
  * chgrp - changes the group associated with a file system object
</b></details>

<details>
<summary>What is sudo? How do you set it up?</summary><br><b>
</b></details>

<details>
<summary>True or False? In order to install packages on the system one must be the root user or use the sudo command</summary><br><b>

True
</b></details>

<details>
<summary>Explain what are ACLs. For what use cases would you recommend to use them?</summary><br><b>
</b></details>

<details>
<summary>You try to create a file but it fails. Name at least three different reason as to why it could happen</summary><br><b>

* No more disk space
* No more inodes
* No permissions
</b></details>

#### Linux systemd

<details>
<summary>What is systemd?</summary><br>
<b>
Systemd is a daemon (System 'd', d stands from daemon).

A daemon is a program that runs in the background without direct control of the user, although the user can at any time
talk to the daemon.

systemd has many features such as user processes control/tracking, snapshot support, inhibitor locks..


If we visualize the unix/linux system in layers, systemd would fall directly after the linux kernel.

Hardware -> Kernel -> <u>Daemons</u>, System Libraries, Server Display.
</b>
</details>

<details>
<summary>On a system which uses systemd, how would you display the logs?</summary><br><b>

<code>journalctl</code>
</b></details>

<details>
<summary>Describe how to make a certain process/app a service</summary><br><b>
</b></details>

##### Linux Debugging

<details>
<summary>Where system logs are located?</summary><br><b>

/var/log
</b></details>

<details>
<summary>How to follow file's content as it being appended without opening the file every time?</summary><br><b>

tail -f <file_name>
</b></details>

<details>
<summary>What are you using for troubleshooting and debugging <b>network</b> issues?</summary><br><b>

<code>dstat -t</code> is great for identifying network and disk issues.
<code>netstat -tnlaup</code> can be used to see which processes are running on which ports.
<code>lsof -i -P</code> can be used for the same purpose as netstat.
<code>ngrep -d any metafilter</code> for matching regex against payloads of packets.
<code>tcpdump</code> for capturing packets
<code>wireshark</code> same concept as tcpdump but with GUI (optional).
</b></details>

<details>
<summary>What are you using for troubleshooting and debugging <b>disk & file system</b> issues?</summary><br><b>

<code>dstat -t</code> is great for identifying network and disk issues.
<code>opensnoop</code> can be used to see which files are being opened on the system (in real time).
</b></details>

<details>
<summary>What are you using for troubleshooting and debugging <b>process</b> issues?</summary><br><b>

<code>strace</code> is great for understanding what your program does. It prints every system call your program executed.
</b></details>

<details>
<summary>What are you using for debugging CPU related issues?</summary><br><b>

<code>top</code> will show you how much CPU percentage each process consumes
<code>perf</code> is a great choice for sampling profiler and in general, figuring out what your CPU cycles are "wasted" on
<code>flamegraphs</code> is great for CPU consumption visualization (http://www.brendangregg.com/flamegraphs.html)
</b></details>

<details>
<summary>You get a call from someone claiming "my system is SLOW". What do you do?</summary><br><b>

* Check with `top` for anything unusual
* Run `dstat -t` to check if it's related to disk or network.
* Check if it's network related with `sar`
* Check I/O stats with `iostat`
</b></details>

<details>
<summary>Explain iostat output</summary><br><b>
</b></details>

<details>
<summary>How to debug binaries?</summary><br><b>
</b></details>

<details>
<summary>What is the difference between CPU load and utilization?</summary><br><b>
</b></details>

<details>
<summary>How you measure time execution of a program?</summary><br><b>
</b></details>

#### Linux Kernel

<details>
<summary>What is a kernel, and what does it do?</summary><br><b>

The kernel is part of the operating system and is responsible for tasks like:

  * Allocating memory
  * Schedule processes
  * Control CPU
</b></details>

<details>
<summary>How do you find out which Kernel version your system is using?</summary><br><b>

`uname -a` command
</b></details>

<details>
<summary>What is a Linux kernel module and how do you load a new module?</summary><br><b>
</b></details>

<details>
<summary>Explain user space vs. kernel space</summary><br><b>

The operating system executes the kernel in protected memory to prevent anyone from changing (and risking it crashing). This is what is known as "Kernel space".
"User space" is where users executes their commands or applications. It's important to create this separation since we can't rely on user applications to not tamper with the kernel, causing it to crash.

Applications can access system resources and indirectly the kernel space by making what is called "system calls".
</b></details>

<details>
<summary>What are system calls? What system calls are you familiar with?</summary><br><b>
</b></details>

#### Linux Virtualization

<details>
<summary>What virtualization solutions are available for Linux?</summary><br><b>
</b></details>

<details>
<summary>What is KVM?</summary><br><b>
</b></details>

#### Linux SSH

<details>
<summary>What is SSH? How to check if a Linux server is running SSH?</summary><br><b>

[Wikipedia Definition](https://en.wikipedia.org/wiki/SSH_(Secure_Shell)): "SSH or Secure Shell is a cryptographic network protocol for operating network services securely over an unsecured network."

[Hostinger.com Definition](https://www.hostinger.com/tutorials/ssh-tutorial-how-does-ssh-work): "SSH, or Secure Shell, is a remote administration protocol that allows users to control and modify their remote servers over the Internet."

An SSH server will have SSH daemon running. Depends on the distribution, you should be able to check whether the service is running (e.g. systemctl status sshd).
</b></details>

<details>
<summary>Why SSH is considered better than telnet?</summary><br><b>

Telnet also allows you to connect to a remote host but as opposed to SSH where the communication is encrypted, in telnet, the data is sent in clear text, so it doesn't considered to be secured because anyone on the network can see what exactly is sent, including passwords.
</b></details>

<details>
<summary>What is stored in <code>~/.ssh/known_hosts</code>?</summary><br><b>
</b></details>

<details>
<summary>You try to ssh to a server and you get "Host key verification failed". What does it mean?</summary><br><b>

It means that the key of the remote host was changed and doesn't match the one that stored on the machine (in ~/.ssh/known_hosts).
</b></details>

<details>
<summary>What is the difference between SSH and SSL?</summary><br><b>
</b></details>

<details>
<summary>What <code>ssh-keygen</code> is used for?</summary><br><b>
</b></details>

<details>
<summary>What is SSH port forwarding?</summary><br><b>
</b></details>

#### Linux - Globbing, Wildcards

<details>
<summary>What is Globbing?</summary><br><b>
</b></details>

<details>
<summary>What are wildcards? Can you give an example of how to use them?</summary><br><b>
</b></details>

<details>
<summary>Explain what will <code>ls [XYZ]</code> match</summary><br><b>
</b></details>

<details>
<summary>Explain what will <code>ls [^XYZ]</code> match</summary><br><b>
</b></details>

<details>
<summary>Explain what will <code>ls [0-5]</code> match</summary><br><b>
</b></details>

<details>
<summary>What each of the following matches

  * ?
  * *</summary><br><b>

  * The ? matches any single character
  * The * matches zero or more characters
</b></details>

<details>
<summary>What do we grep for in each of the following commands?:

  * <code>grep '[0-9]\{1,3\}\.[0-9]\{1,3\}\.[0-9]\{1,3\}\.[0-9]\{1,3\}' some_file</code>
  * <code>grep -E "error|failure" some_file</code>
  * <code>grep '[0-9]$' some_file</code>
</summary><br><b>

1. An IP address
2. The word "error" or "failure"
3. Lines which end with a number
</b></details>

<details>
<summary>Which line numbers will be printed when running `grep '\baaa\b'` on the following content:

aaa
bbb
ccc.aaa
aaaaaa</summary><br><b>

lines 1 and 3.
</b></details>

<details>
<summary>What is the difference single and double quotes?</summary><br><b>
</b></details>

<details>
<summary>What is escaping? What escape character is used for escaping?</summary><br><b>
</b></details>

<details>
<summary>What is an exit code? What exit codes are you familiar with?</summary><br><b>

An exit code (or return code) represents the code returned by a child process to its
parent process.

0 is an exit code which represents success while anything higher than 1 represents error.
Each number has different meaning, based on how the application was developed.

I consider this as a good blog post to read more about it: https://shapeshed.com/unix-exit-codes
</b></details>

#### Linux Boot Process

<details>
<summary>Tell me everything you know about the Linux boot process</summary><br><b>

Another way to ask this: what happens from the moment you turned on the server until you get a prompt
</b></details>

<details>
<summary>What is GRUB2?</summary><br><b>
</b></details>

<details>
<summary>What is Secure Boot?</summary><br><b>
</b></details>

<details>
<summary>What can you find in /boot?</summary><br><b>
</b></details>

##### Linux Disk & Filesystem

<details>
<summary>What's an inode?</summary><br><b>

For each file (and directory) in Linux there is an inode, a data structure which stores meta data
related to the file like its size, owner, permissions, etc.
</b></details>

<details>
<summary>Which of the following is not included in inode:

  * Link count
  * File size
  * File name
  * File timestamp</summary><br><b>

File name (it's part of the directory file)
</b></details>

<details>
<summary>How to check which disks are currently mounted?</summary><br><b>

Run `mount`
</b></details>

<details>
<summary>You run the <code>mount</code> command but you get no output. How would you check what mounts you have on your system?</summary><br><b>

`cat /proc/mounts`
</b></details>

<details>
<summary>What is the difference between a soft link and hard link?</summary><br><b>

Hard link is the same file, using the same inode.
Soft link is a shortcut to another file, using a different inode.
</b></details>

<details>
<summary>True or False? You can create an hard link for a directory</summary><br><b>

False
</b></details>

<details>
<summary>True or False? You can create a soft link between different filesystems</summary><br><b>

True
</b></details>

<details>
<summary>What happens when you delete the original file in case of soft link and hard link?</summary><br><b>
</b></details>

<details>
<summary>Can you check what type of filesystem is used in /home?</summary><br><b>

There are many answers for this question. One way is running `df -T`
</b></details>

<details>
<summary>What is a swap partition? What is it used for?</summary><br><b>
</b></details>

<details>
<summary>How to create a

  * new empty file
  * a file with text (without using text editor)
  * a file with given size</summary><br><b>
</b></details>

<details>
<summary>You are trying to create a new file but you get "File system is full". You check with df for free space and you see you used only 20% of the space. What could be the problem?</summary><br><b>
</b></details>

<details>
<summary>How would you check what is the size of a certain directory?</summary><br><b>

`du -sh`
</b></details>

<details>
<summary>What is LVM?</summary><br><b>
</b></details>

<details>
<summary>Explain the following in regards to LVM:

  * PV
  * VG
  * LV</summary><br><b>


</b></details>

<details>
<summary>What is NFS? What is it used for?</summary><br><b>
</b></details>

<details>
<summary>What RAID is used for? Can you explain the differences between RAID 0, 1, 5 and 10?</summary><br><b>
</b></details>

<details>
<summary>Describe the process of extending a filesystem disk space</summary><br><b>
</b></details>

<details>
<summary>What is lazy umount?</summary><br><b>
</b></details>

<details>
<summary>What is tmpfs?</summary><br><b>
</b></details>

<details>
<summary>What is stored in each of the following logs?

  * /var/log/messages
  * /var/log/boot.log</summary><br><b>
</b></details>

<details>
<summary>True or False? both /tmp and /var/tmp cleared upon system boot</summary><br><b>

False. /tmp is cleared upon system boot while /var/tmp is cleared every a couple of days or not cleared at all (depends on distro).
</b></details>

#### Linux Performance Analysis

<details>
<summary>How to check what is the current load average?</summary><br><b>

One can use `uptime` or `top`
</b></details>

<details>
<summary>You know how to see the load average, great. but what each part of it means? for example 1.43, 2.34, 2.78</summary><br><b>

[This article](http://www.brendangregg.com/blog/2017-08-08/linux-load-averages.html) summarizes the load average topic in a great way
</b></details>

<details>
<summary>How to check process usage?</summary><br><b>

pidstat
</b></details>

<details>
<summary>How to check disk I/O?</summary><br><b>

`iostat -xz 1`
</b></details>

<details>
<summary>How to check how much free memory a system has? How to check memory consumption by each process?</summary><br><b>

You can use the commands <code>top</code> and <code>free</code>
</b></details>

<details>
<summary>How to check TCP stats?</summary><br><b>

sar -n TCP,ETCP 1
</b></details>

#### Linux Processes

<details>
<summary>how to list all the processes running in your system?</summary><br><b>

`ps -ef`
</b></details>

<details>
<summary>How to run a process in the background and why to do that in the first place?</summary><br><b>

You can achieve that by specifying & at the end of the command.
As to why, since some commands/processes can take a lot of time to finish
execution or run forever, you may want to run them in the background instead of waiting for them to finish before gaining control again in current session.
</b></details>

<details>
<summary>How can you find how much memory a specific process consumes?</summary><br><b>
</b></details>

<details>
<summary>What signal is used by default when you run 'kill *process id*'?</summary><br><b>
<pre>
The default signal is SIGTERM (15). This signal kills
process gracefully which means it allows it to save current
state configuration.
</pre>
</b></details>

<details>
<summary>What signals are you familiar with?</summary><br><b>

SIGTERM - default signal for terminating a process
SIGHUP - common usage is for reloading configuration
SIGKILL - a signal which cannot caught or ignored

To view all available signals run `kill -l`
</b></details>

<details>
<summary>What <code>kill 0</code> does?</summary><br><b>
</b></details>

<details>
<summary>What <code>kill -0 <PID></code> does?</summary><br><b>
</b></details>

<details>
<summary>What is a trap?</summary><br><b>
</b></details>

<details>
<summary>Every couple of days, a certain process stops running. How can you look into why it's happening?</summary><br><b>
</b></details>

<details>
<summary>What happens when you press ctrl + c?</summary><br><b>
</b></details>

<details>
<summary>What is a Daemon in Linux?</summary><br><b>

A background process. Most of these processes are waiting for requests or set of conditions to be met before actually running anything.
Some examples: sshd, crond, rpcbind.
</b></details>

<details>
<summary>What are the possible states of a process in Linux?</summary><br><b>
<pre>
Running (R)
Uninterruptible Sleep (D) - The process is waiting for I/O
Interruptible Sleep (S)
Stopped (T)
Dead (x)
Zombie (z)
</pre>
</b></details>

<details>
<summary>How do you kill a process in D state?</summary><br><b>
</b></details>

<details>
<summary>What is a zombie process?</summary><br><b>

A process which has finished to run but has not exited.

One reason it happens is when a parent process is programmed incorrectly. Every parent process should execute wait() to get the exit code from the child process which finished to run. But when the parent isn't checking for the child exit code, the child process can still exists although it finished to run.
</b></details>

<details>
<summary>How to get rid of zombie processes?</summary><br><b>

You can't kill a zombie process the regular way with `kill -9` for example as it's already dead.

One way to kill zombie process is by sending SIGCHLD to the parent process telling it to terminate its child processes. This might not work if the parent process wasn't programmed properly. The invocation is `kill -s SIGCHLD [parent_pid]`

You can also try closing/terminating the parent process. This will make the zombie process a child of init (1) which does periodic cleanups and will at some point clean up the zombie process.
</b></details>

<details>
<summary>How to find all the

  * Processes executed/owned by a certain user
  * Process which are Java processes
  * Zombie Processes
</summary><br><b>

If you mention at any point ps command with arugments, be familiar with what these arguments does exactly.
</b></details>

<details>
<summary>What is the init process?</summary><br><b>
It is the first process executed by the kernel during the booting of a system. It is a daemon process which runs till the system is shutdown. That is why, it is the parent of all the processes
</b></details>

<details>
<summary>Can you describe how processes are being created?</summary><br><b>
</b></details>

<details>
<summary>How to change the priority of a process? Why would you want to do that?</summary><br><b>
</b></details>

<details>
<summary>Can you explain how network process/connection is established and how it's terminated?></summary><br></b>
</b></details>

<details>
<summary>What <code>strace</code> does? What about <code>ltrace</code>?</summary><br><b>
</b></details>

<details>
<summary>Find all the files which end with '.yml' and replace the number 1 in 2 in each file</summary><br><b>

find /some_dir -iname \*.yml -print0 | xargs -0 -r sed -i "s/1/2/g"
</b></details>

<details>
<summary>You run ls and you get "/lib/ld-linux-armhf.so.3 no such file or directory". What is the problem?</summary><br><b>

The ls executable is built for an incompatible architecture.
</b></details>

<details>
<summary>How would you split a 50 lines file into 2 files of 25 lines each?</summary><br><b>

You can use the <code>split</code> command this way: <code>split -l 25 some_file</code>
</b></details>

<details>
<summary>What is a file descriptor? What file descriptors are you familiar with?</summary><br><b>
Kerberos
File descriptor, also known as file handler, is a unique number which identifies an open file in the operating system.

In Linux (and Unix) the first three file descriptors are:

  * 0 - the default data stream for input
  * 1 - the default data stream for output
  * 2 - the default data stream for output related to errors

This is a great article on the topic: https://www.computerhope.com/jargon/f/file-descriptor.htm
</b></details>

<details>
<summary>What is NTP? What is it used for?</summary><br><b>
</b></details>

<details>
<summary>Explain Kernel OOM</summary><br><b>
</b></details>

##### Linux Security

<details>
<summary>What is chroot? In what scenarios would you consider using it?</summary><br><b>
</b></details>

<details>
<summary>What is SELiunx?</summary><br><b>
</b></details>

<details>
<summary>What is Kerberos?</summary><br><b>
</b></details>

<details>
<summary>What is nftables?</summary><br><b>
</b></details>

<details>
<summary>What firewalld daemon is responsible for?</summary><br><b>
</b></details>

<details>
<summary>Do you have experience with hardening servers? Can you describe the process?</summary><br><b>
</b></details>

##### Linux Networking

<details>
<summary>How to list all the interfaces?</summary><br><b>
</b></details>

<details>
<summary>What is the loopback (lo) interface?</summary><br><b>
</b></details>

<details>
<summary>What the following commands are used for?

  * ip addr
  * ip route
  * ip link
  * ping
  * netstat
  * traceroute</summary><br><b>
</b></details>

<details>
<summary>What is a network namespace? What is it used for?</summary><br><b>
</b></details>

<details>
<summary>How to check if a certain port is being used?</summary><br><b>

One of the following would work:

```
netstat -tnlp | grep <port_number>
lsof -i -n -P | grep <port_number>
```
</b></details>

<details>
<summary>How can you turn your Linux server into a router?</summary><br><b>
</b></details>

<details>
<summary>What is a virtual IP? In what situation would you use it?</summary><br><b>
</b></details>

<details>
<summary>True or False? The MAC address of an interface is assigned/set by the OS</summary><br><b>

False
</b></details>

<details>
<summary>Can you have more than one default gateway in a given system?</summary><br><b>

Technically, yes.
</b></details>

<details>
<summary>Which port is used in each of the following protocols?:

  * SSH
  * SMTP
  * HTTP
  * DNS
  * HTTPS
</summary><br><b>

  * SSH - 22
  * SMTP - 35
  * HTTP - 80
  * DNS - 53
  * HTTPS - 443
</b></details>

<details>
<summary>What is telnet and why is it a bad idea to use it in production? (or at all)</summary><br><b>
</b></details>

<details>
<summary>What is the routing table? How do you view it?</summary><br><b>
</b></details>

<details>
<summary>How can you send an HTTP request from your shell?</summary><br><b>
<br>
Using nc is one way<br>
</b></details>

<details>
<summary>What are packet sniffers? Have you used one in the past? If yes, which packet sniffers have you used and for what purpose?</summary><br><b>
It is a network utility that analyses and may inject tasks into the data-stream travelling over the targeted network.
</b></details>

<details>
<summary>How to list active connections?</summary><br><b>
</b></details>

<details>
<summary>How to trigger neighbor discovery in IPv6?</summary><br><b>

One way would be `ping6 ff02::1`
</b></details>

<details>
<summary>What is network interface bonding and do you know how it's performed in Linux?</summary><br><b>
</b></details>

<details>
<summary>What network bonding modes are there?</summary><br><b>

There a couple of modes:

  * balance-rr: round robing bonding
  * active-backup: a fault tolerance mode where only one is active
  * balance-tlb: Adaptive transmit load balancing
  * balance-alb: Adaptive load balancing
</b></details>

<details>
<summary>What is a bridge? How it's added in Linux OS?</summary><br><b>
</b></details>

##### Linux DNS

<details>
<summary>How to check what is the hostname of the system?</summary><br><b>

`cat /etc/hostname`

You can also run `hostnamectl` or `hostname` but that might print only a temporary hostname. The one in the file is the permanent one.
</b></details>

<details>
<summary>What the file <code>/etc/resolv.conf</code> is used for? What does it include?</summary><br><b>
</b></details>

<details>
<summary>What commands are you using for performing DNS queries (or troubleshoot DNS related issues)?</summary><br><b>

You can specify one or more of the following:

 * <code>dig</code>
 * <code>host</code>
 * <code>nslookup</code>
</b></details>

##### Linux Packaging

<details>
<summary>Do you have experience with packaging? (as in building packages) Can you explain how does it works?</summary><br><b>
</b></details>

<details>
<summary>How packages installation/removal is performed on the distribution you are using?</summary><br><b>

The answer depends on the distribution being used.

In Fedora/CentOS/RHEL/Rocky it can be done with `rpm` or `dnf` commands.
In Ubuntu it can be done with the `apt` command.
</b></details>

<details>
<summary>RPM: explain the spec format (what it should and can include)</summary><br><b>
</b></details>

<details>
<summary>How do you list the content of a package without actually installing it?</summary><br><b>
</b></details>

<details>
<summary>How to know to which package a file on the system belongs to? Is it a problem if it doesn't belongs to any package?</summary><br><b>
</b></details>

<details>
<summary>Where repositories are stored? (based on the distribution you are using)</summary><br><b>
</b></details>

<details>
<summary>What is an archive? How do you create one in Linux?</summary><br><b>
</b></details>

<details>
<summary>How to extract the content of an archive?</summary><br><b>
</b></details>

<details>
<summary>Why do we need package managers? Why not simply creating archives and publish them?</summary><br><b>

Package managers allow you to manage packages lifecycle as in installing, removing and updating the packages.<br>
In addition, you can specify in a spec how a certain package will be installed - where to copy the files, which commands to run prior to the installation, post the installation, etc.
</b></details>

#### Linux DNF

<details>
<summary>How to look for a package that provides the command /usr/bin/git? (the package isn't necessarily installed)</summary><br><b>

dnf provides /usr/bin/git
</b></details>

##### Linux Applications and Services

<details>
<summary>What can you find in /etc/services?</summary><br><b>
</b></details>

<details>
<summary>How to make sure a Service starts automatically after a reboot or crash?</summary><br><b>

Depends on the init system.

Systemd: <code> systemctl enable [service_name] </code>
System V: <code> update-rc.d [service_name] </code> and add this line <code> id:5678:respawn:/bin/sh /path/to/app </code> to /etc/inittab
Upstart: add Upstart init script at /etc/init/service.conf
</b></details>

<details>
<summary>You run <code>ssh 127.0.0.1</code> but it fails with "connection refused". What could be the problem?</summary><br><b>

1. SSH server is not installed
2. SSH server is not running
</b></details>

<details>
<summary>How to print the shared libraries required by a certain program? What is it useful for?</summary><br><b>
</b></details>

<details>
<summary>What is CUPS?</summary><br><b>
</b></details>

<details>
<summary>What types of web servers are you familiar with?</summary><br><b>

Nginx, Apache httpd.
</b></details>

##### Linux Users and Groups

<details>
<summary>What is a "superuser" (or root user)? How is it different from regular users?</summary><br><b>
</b></details>

<details>
<summary>How do you create users? Where user information is stored?</summary><br><b>
</b></details>

<details>
<summary>Which file stores information about groups?</summary><br><b>
</b></details>

<details>
<summary>How do you change/set the password of a user?</summary><br><b>
</b></details>

<details>
<summary>Which file stores users passwords? Is it visible for everyone?</summary><br><b>
</b></details>

<details>
<summary>Do you know how to create a new user without using adduser/useradd command?</summary><br><b>
</b></details>

<details>
<summary>What information is stored in /etc/passwd? explain each field</summary><br><b>
</b></details>

<details>
<summary>How to add a new user to the system without providing him the ability to log-in into the system?</summary><br><b>

`adduser user_name --shell=/bin/false --no-create-home`
You can also add a user and then edit /etc/passwd.
</b></details>

<details>
<summary>How to switch to another user? How to switch to the root user?</summary><br><b>

su command.
Use su - to switch to root
</b></details>

<details>
<summary>What is the UID the root user? What about a regular user?</summary><br><b>
</b></details>

<details>
<summary>What can you do if you lost/forogt the root password?</summary><br><b>

Re-install the OS IS NOT the right answer :)
</b></details>

<details>
<summary>What is /etc/skel?</summary><br><b>
</b></details>

<details>
<summary>How to see a list of who logged-in to the system?</summary><br><b>

Using the `last` command.
</b></details>

<details>
<summary>Explain what each of the following commands does:

  * useradd
  * usermod
  * whoami
  * id</summary><br><b>
</b></details>

#### Linux Hardware

<details>
<summary>Where can you find information on the processor?</summary><br><b>

/proc/cpuinfo
</b></details>

<details>
<summary>How can you print information on the BIOS, motherboard, processor and RAM?</summary><br><b>

dmidecoode
</b></details>

<details>
<summary>How can you print all the information on connected block devices in your system?</summary><br><b>

lsblk
</b></details>

#### Linux - Random

<details>
<summary>Give 5 commands which are two letters long</summary><br><b>

ls, wc, dd, df, du, ps, ip, cp, cd ...
</b></details>

<details>
<summary>What ways are there for creating a new empty file?</summary><br><b>

  * touch new_file
  * echo "" > new_file
</b></details>

<details>
<summary>How `cd -` works? How does it knows the previous location?</summary><br><b>

$OLDPWD
</b></details>

<details>
<summary>List three ways to print all the files in the current directory</summary><br><b>

* ls
* find .
* echo *
</b></details>

<details>
<summary>How to count the number of lines in a file? What about words?</summary><br><b>
</b></details>

<details>
<summary>You define x=2 in /etc/bashrc and x=6 ~/.bashrc you then login to the system. What would be the value of x?</summary><br><b>
</b></details>

<details>
<summary>What is the difference between man and info?</summary><br><b>

A good answer can be found [here](https://askubuntu.com/questions/9325/what-is-the-difference-between-man-and-info-documentation)
</b></details>

<details>
<summary>Explain "environment variables". How do you list all environment variables?</summary><br><b>
</b></details>

<details>
<summary>How to create your own environment variables?</summary><br><b>

`X=2` for example. But this will persist to new shells. To have it in new shells as well, use `export X=2`
</b></details>

<details>
<summary>What a double dash (--) mean?</summary><br><b>

It's used in commands to mark the end of commands options. One common example is when used with git to discard local changes: `git checkout -- some_file`
</b></details>

#### Linux - AWK

<details>
<summary>What the <code>awk</code> command does? Have you used it? What for?</summary><br><b>

From Wikipedia: "AWK is domain-specific language designed for text processing and typically used as a data extraction and reporting tool"
</b></details>

<details>
<summary>How to print the 4th column in a file?</summary><br><b>

`awk '{print $4}' file`
</b></details>

<details>
<summary>How to print every line that is longer than 79 characters?</summary><br><b>

`awk 'length($0) > 79' file`
</b></details>

<details>
<summary>What the <code>lsof</code> command does? Have you used it? What for?</summary><br><b>
</b></details>

<details>
<summary>What is the difference between find and locate?</summary><br><b>
</b></details>

#### System Calls

<details>
<summary>Explain the fork() system call</summary><br><b>

fork() is used for creating a new process. It does so by cloning the calling process but the child process has its own PID and any memory locks, I/O operations and semaphores are not inherited.
</b></details>

<details>
<summary>Explain the exec() system call</summary><br><b>
</b></details>

<details>
<summary>What system call is used for listing files?</summary><br><b>
</b></details>

<details>
<summary>What system call is used for creating a new process?</summary><br><b>
</b></details>

<details>
<summary>What are the differences between exec() and fork()?</summary><br><b>
</b></details>

<details>
<summary>Why do we need the wait system call?</summary><br><b>

wait() is used by a parent process to wait for the child process to finish execution.
If wait is not used by a parent process then a child process might become a zombie process.
</b></details>

<details>
<summary>What execve() does?</summary><br><b>

Executes a program. The program is passed as a filename (or path) and must be a binary executable or a script.
</b></details>

<details>
<summary>What is the return value of malloc?</summary><br><b>
</b></details>

<details>
<summary>Explain the pipe() system call. What does it used for?</summary><br><b>

[Unix pipe implementation](https://toroid.org/unix-pipe-implementation)

"Pipes provide a unidirectional interprocess communication channel. A pipe has a read end and a write end. Data written to the write end of a pipe can be read from the read end of the pipe.
A pipe is created using pipe(2), which returns two file descriptors, one referring to the read end of the pipe, the other referring to the write end."
</b></details>

<details>
<summary>What happens when you execute <code>ls -l</code>?</summary><br><b>

* Shell reads the input using getline() which reads the input file stream and stores into a buffer as a string
* The buffer is broken down into tokens and stored in an array this way: {"ls", "-l", "NULL"}
* Shell checks if an expansion is required (in case of ls *.c)

* Once the program in memory, its execution starts. First by calling readdir()

Notes:

* getline() originates in GNU C library and used to read lines from input stream and stores those lines in the buffer
</b></details>

<details>
<summary>What happens when you execute <code>ls -l *.log</code>?</summary><br><b>
</b></details>

<details>
<summary>What readdir() system call does?</summary><br><b>
</b></details>

<details>
<summary>What exactly the command <code>alias x=y</code> does?</summary><br><b>
</b></details>

#### Linux Filesystem & Files

<details>
<summary>How to create a file of a certain size?</summary><br><b>

There are a couple of ways to do that:

  * dd if=/dev/urandom of=new_file.txt bs=2MB count=1
  * truncate -s 2M new_file.txt
  * fallocate -l 2097152 new_file.txt
</b></details>

<details>
<summary>What does the following block do?:

```
open("/my/file") = 5
read(5, "file content")
```
</summary><br><b>

These system calls are reading the file <code>/my/file</code> and 5 is the file descriptor number.
</b></details>

<details>
<summary>Describe three different ways to remove a file (or its content)</summary><br><b>
</b></details>

<details>
<summary>What is the difference between a process and a thread?</summary><br><b>
</b></details>

<details>
<summary>What is context switch?</summary><br><b>

From [wikipedia](https://en.wikipedia.org/wiki/Context_switch): a context switch is the process of storing the state of a process or thread, so that it can be restored and resume execution at a later point
</b></details>

<details>
<summary>You found there is a server with high CPU load but you didn't find a process with high CPU. How is that possible?</summary><br><b>
</b></details>

##### Linux Advanced - Networking

<details>
<summary>When you run <code>ip a</code> you see there is a device called 'lo'. What is it and why do we need it?</summary><br><b>
</b></details>

<details>
<summary>What the <code>traceroute</code> command does? How does it works?</summary><br><b>

Another common way to task this questions is "what part of the tcp header does traceroute modify?"
</b></details>

<details>
<summary>What is network bonding? What types are you familiar with?</summary><br><b>
</b></details>

<details>
<summary>How to link two separate network namespaces so you can ping an interface on one namespace from the second one?</summary><br><b>
</b></details>

<details>
<summary>What are cgroups?</summary><br><b>
</b></details>

<details>
<summary>Explain Process Descriptor and Task Structure</summary><br><b>
</b></details>

<details>
<summary>What are the differences between threads and processes?</summary><br><b>
</b></details>

<details>
<summary>Explain Kernel Threads</summary><br><b>
</b></details>

<details>
<summary>What happens when socket system call is used?</summary><br><b>

This is a good article about the topic: https://ops.tips/blog/how-linux-creates-sockets
</b></details>

<details>
<summary>You executed a script and while still running, it got accidentally removed. Is it possible to restore the script while it's still running?</summary><br><b>
</b></details>

#### Linux Memory

<details>
<summary>What is the difference between MemFree and MemAvailable in /proc/meminfo?</summary><br><b>

MemFree - The amount of unused physical RAM in your system
MemAvailable - The amount of available memory for new workloads (without pushing system to use swap) based on MemFree, Active(file), Inactive(file), and SReclaimable.
</b></details>

<details>
<summary>What is virtual memory?</summary><br><b>
</b></details>

<details>
<summary>What is the difference between paging and swapping?</summary><br><b>
</b></details>

<details>
<summary>Explain what is OOM killer</summary><br><b>
</b></details>

#### Distribution

<details>
<summary>What is a Linux distribution?</summary><br><b>
</b></details>

<details>
<summary>What Linux distributions are you familiar with?</summary><br><b>
</b></details>

<details>
<summary>What are the components of a Linux distribution?</summary><br><b>

* Kernel
* Utilities
* Services
* Software/Packages Management
</b></details>

#### Linux Advanced - Misc

<details>
<summary>Wildcards are implemented on user or kernel space?</summary><br><b>
</b></details>

<details>
<summary>If I plug a new device into a Linux machine, where on the system, a new device entry/file will be created?</summary><br><b>

/dev
</b></details>

<details>
<summary>Why there are different sections in man? What is the difference between the sections?</summary><br><b>
</b></details>

#### Linux Master Application

A completely free application for testing your knowledge on Linux

<a href="https://play.google.com/store/apps/details?id=com.codingshell.linuxmaster"><img src="images/linux_master.jpeg"/></a>

