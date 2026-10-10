# linuxtask.md
LINUX FUNDAMENTALS

STUDY GUIDE

1. Linux Fundamentals

What is Linux, and why is it widely used?

Linux is an open-source operating system kernel that was created by Linus Torvalds in 1991. It is commonly used to refer to operating systems built around the Linux kernel, known as Linux distributions.

Linux is widely used because it is free, secure, reliable and flexible. It allows users to study and modify its source code, supports different types of computer devices, and provides powerful command-line tools for running commands and automating tasks. It is also widely used in servers, cloud computing, software development and cybersecurity.

What is the difference between the Linux kernel and a Linux distribution?

The Linux kernel is the central part of the operating system. It manages the computer's hardware, memory, processes and other system resources.

A Linux distribution is a complete operating system built around the Linux kernel. It includes the kernel, system utilities, applications, a package manager and other tools needed to use the computer.

For example, Ubuntu, Debian and Fedora are Linux distributions, while the Linux kernel is the core component they use.

Name three popular Linux distributions and their primary uses.

Ubuntu is a popular Linux distribution used for personal computers, servers and software development. It is also suitable for beginners.

Debian is known for its stability and reliability. It is commonly used on servers and as the foundation for other Linux distributions.

Fedora is a Linux distribution that provides modern features and software. It is commonly used by developers and people who want to work with newer Linux technologies.

2. Linux Filesystem

What is the purpose of the root directory ("/")?

The root directory is the main directory in a Linux filesystem. All other directories and files are organised under it. It is represented by a forward slash ("/") and serves as the starting point for absolute file paths.

What is the difference between "/home" and "/root"?

The "/home" directory contains the personal directories of regular users. For example, a user named John may have a home directory at "/home/john".

The "/root" directory is the personal home directory of the root user, who has administrative privileges on the system. Therefore, "/home" is mainly for regular users, while "/root" is for the system administrator.

Which directory stores system configuration files?

The "/etc" directory stores most system-wide configuration files. These files control different aspects of the operating system and its services. Examples include "/etc/passwd", which contains user account information, and "/etc/hostname", which stores the system's hostname.

Which directory stores most log files?

The "/var/log" directory stores many system and application log files. These logs record events, errors and other activities that help administrators troubleshoot problems and monitor system performance.

3. Navigation and File Management

Which command displays the current directory?

The "pwd" command displays the full path of the directory the user is currently working in. For example, typing "pwd" may display "/home/john".

Which command changes directories?

The "cd" command is used to move from one directory to another. For example, "cd /etc" moves the user to the "/etc" directory, while "cd .." moves one level up. The command "cd ~" takes the user to their home directory.

Which command lists the contents of a directory?

The "ls" command displays the files and directories in a specified location. The command "ls -l" displays detailed information, while "ls -a" also displays hidden files. The command "ls -lh" displays file sizes in a more readable format.

How do you create a new directory?

The "mkdir" command is used to create a new directory. For example, "mkdir documents" creates a directory named "documents". The option "mkdir -p" can be used to create a directory together with any missing parent directories.

How do you create an empty file?

The "touch" command is commonly used to create an empty file. For example, "touch notes.txt" creates a file named "notes.txt" if it does not already exist. If the file exists, the command updates its timestamps.

Which commands are used to copy, move and delete files?

The "cp" command is used to copy files, while "mv" is used to move or rename them. The "rm" command deletes files. For example, "cp notes.txt backup.txt" copies a file, "mv notes.txt report.txt" renames it, and "rm notes.txt" deletes it. The "rm -r" command can remove directories and their contents, so it should be used carefully.

4. Searching

What is the difference between "find" and "grep"?

The "find" command searches for files and directories based on conditions such as their names, sizes and modification dates. The "grep" command searches for specific words or patterns inside files.

For example, "find /home -name "*.txt"" searches for text files under "/home", while "grep "error" log.txt" searches for lines containing the word "error" in "log.txt".

Which command searches for files?

The "find" command is used to search for files and directories. For example, "find /home -name "notes.txt"" searches for a file named "notes.txt" under the "/home" directory.

Which command searches inside files?

The "grep" command searches the contents of files for specific words or patterns. For example, "grep "Linux" notes.txt" displays lines containing the word "Linux". The "grep -i" option makes the search case-insensitive.

How do wildcards help when searching?

Wildcards are special characters used to match filenames or groups of files. The asterisk ("*") represents any number of characters, while the question mark ("?") represents exactly one character.

For example, "ls *.txt" displays files ending in ".txt", while "ls file?.txt" can match names such as "file1.txt" and "fileA.txt".

5. Basic Commands

What does the "echo" command do?

The "echo" command displays text or variable values on the terminal. It can also be used with redirection to write text into a file. For example, "echo "Hello"" displays the word "Hello", while "echo "Hello" > notes.txt" writes the text into a file named "notes.txt".

What is the purpose of the "history" command?

The "history" command displays previously entered commands in the shell. It helps users review commands they have used and repeat earlier operations when necessary. For example, "history 10" displays the ten most recent entries in the history list.

What does the pipe ("|") operator do?

The pipe operator passes the output of one command as input to another command. This allows users to combine commands to perform tasks more efficiently. For example, "ls | grep ".txt"" passes the output of "ls" to "grep", which searches for matching lines.

What is the difference between ">" and ">>"?

The ">" operator redirects output into a file and replaces its existing contents. If the file does not exist, it creates one.

The ">>" operator also redirects output, but it adds the new content to the end of the file without removing the existing contents.

How can you access a command's manual page?

The "man" command displays the manual page for a Linux command. For example, "man ls" displays information about the "ls" command, including its purpose and available options. Users can also use the "--help" option with many commands to view a brief explanation of how they work.

6. Users and Groups

What is the difference between a regular user and the root user?

A regular user has limited permissions and can generally access their own files and perform normal activities. The root user has administrative privileges and can make changes to almost every part of the system.

Regular accounts are safer for everyday activities because mistakes made by the root user can affect the entire system.

What is a group?

A group is a collection of user accounts that share certain access permissions. Groups make it easier to manage access to files and resources without setting permissions separately for every user. For example, a group called "developers" may be given permission to access project files.

What does the "sudo" command do?

The "sudo" command allows an authorised user to execute a command with the privileges of another user, usually the root user. It is commonly used to perform administrative tasks, such as installing software or updating the system. For example, "sudo apt update" updates the package information on systems that use APT.

Which command displays information about the current user?

The "whoami" command displays the username of the current user. The "id" command provides more information, including the user's ID, primary group and supplementary groups.

7. Permissions

What do the "r", "w" and "x" permissions represent?

The letters "r", "w" and "x" represent read, write and execute permissions.

For a file, read permission allows the user to view its contents, write permission allows the user to modify it, and execute permission allows the file to be run as a program or script.

For a directory, read permission allows the user to list its contents, write permission allows the user to create or remove entries, and execute permission allows the user to enter the directory and access files by name, subject to other permissions.

What is the difference between file ownership and group ownership?

File ownership identifies the user who owns a file, while group ownership identifies the group associated with it. Linux uses ownership and permissions to determine which users can access or modify files.

The "chown" command can change a file's owner, while "chgrp" can change its group.

Which command changes file permissions?

The "chmod" command is used to change file and directory permissions. For example, "chmod 755 script.sh" gives the owner read, write and execute permissions, while the group and other users receive read and execute permissions.

Another example is "chmod 644 notes.txt", which gives the owner read and write permissions while giving the group and other users read permission.

Which command changes file ownership?

The "chown" command changes the ownership of a file or directory. For example, "chown john notes.txt" changes the owner of "notes.txt" to John, provided the command is run with the required privileges. The "chgrp" command changes the group associated with a file.

8. Important System Files

What information is stored in "/etc/passwd"?

The "/etc/passwd" file contains basic information about user accounts on a Linux system. Each entry includes the username, user ID, primary group ID, account description, home directory and login shell. It commonly contains an "x" in the password field because password hashes are usually stored separately in "/etc/shadow".

Why is "/etc/shadow" protected?

The "/etc/shadow" file stores password hashes and password-aging information. It is protected because unauthorised access to password hashes could allow attackers to attempt offline password-cracking attacks. Access is therefore restricted to root and authorised system processes.

What is the purpose of "/var/log"?

The "/var/log" directory stores logs generated by the operating system and applications. These logs help administrators identify errors, investigate security incidents, troubleshoot services and monitor system activities.

Which file stores the system hostname?

The "/etc/hostname" file normally stores the system's hostname. A hostname is the name used to identify a computer on a network. The hostname can be viewed or changed using appropriate system commands, such as "hostnamectl" on systems that support it.

9. Installation Basics

What is a partition?

A partition is a section of a storage device, such as a hard drive or SSD, that is treated as a separate storage area. Partitions can be used to organise system files, user data and other information. They can also help support different operating systems on the same computer.

What is a filesystem?

A filesystem is the method an operating system uses to organise, store and retrieve files on a storage device. It manages file names, directories, permissions and information about available storage space.

Examples of Linux filesystems include ext4, XFS and Btrfs. Windows filesystems such as NTFS and exFAT can also be accessed on Linux systems when the necessary support is available.

What is the purpose of the swap partition?

A swap partition is an area of storage used as virtual memory. It allows Linux to move less-active memory pages from RAM to storage, helping the system manage memory when RAM is under pressure. Swap can also support hibernation when configured appropriately.

Swap may be created as a dedicated partition or as a swap file.

Why is ext4 commonly used?

Ext4, which stands for Fourth Extended Filesystem, is widely used in Linux because it is stable, reliable and offers good performance. It supports journaling, which helps the filesystem recover more easily after certain system crashes. It also handles different file sizes efficiently and is supported by many Linux distributions.

These features make ext4 a suitable choice for general-purpose Linux installations.
