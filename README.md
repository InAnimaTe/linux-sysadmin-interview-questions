Linux System Administrator/DevOp Interview Questions
====================================================

A collection of linux sysadmin/devop interview questions. Feel free to contribute via pull requests, issues or email messages.

##### This originated from /chassing. Adding as much as much as I can to it.

## <a name='toc'>Table of Contents</a>

  1. [Contributors](#contributors)
  1. [General Questions](#general)
  1. [Simple Linux Questions](#simple)
  1. [Medium Linux Questions](#medium)
  1. [Hard Linux Questions](#hard)
  1. [Expert Linux Questions](#expert)
  1. [Networking Questions](#network)
  1. [General Front-end Questions](#web)
  1. [DevOp Questions](#devop)
  1. [Fun Questions](#fun)
  1. [Demo Time](#demo)
  1. [Other Great References](#references)


####[[⬆]](#toc) <a name='contributors'>Contributors:</a>

* [moregeek](https://github.com/moregeek)
* [typhonius](https://github.com/typhonius)
* martin
* [negesti](https://github.com/negesti)
* peter
* [andreashappe](https://github.com/andreashappe)
* [quatrix](https://github.com/quatrix)
* [biyanisuraj](https://github.com/biyanisuraj)

The majority of the questions were collected from:

* https://github.com/gurmeet1109/docgurmeet/tree/master/InterviewQuestionsSamples
* https://github.com/kylejohnson/linux-sysadmin-interview-questions/blob/master/test.md


####[[⬆]](#toc) <a name='general'>General Questions:</a>

* What did you learn yesterday/this week?
* Talk about your preferred development/administration environment. (OS, Editor, Browsers, Tools etc.)
* Tell me about the last major Linux project you finished.
* Tell me about the biggest mistake you've made in [some recent time period] and how you would do it differently today. What did you learn from this experience?
* What function does DNS play on a network?
* What is HTTP?
* What is an HTTP proxy and how does it work?
* What is SMTP? Give the basic scenario of how a mail message is delivered via SMTP!
* What is RAID? What is RAID0, RAID1, RAID5, RAID10?
* What is a level 0 backup? What is an incremental backup?
* Describe the general file system hierarchy of a Linux system.


####[[⬆]](#toc) <a name='simple'>Simple Linux Questions:</a>

* What is the name and the UID of the administrator user?
* How to list all files, including hidden one, in a directory?
* What is the Unix/Linux command to remove a directory and its contents?
* Which command will show you free/used memory? Does free memory exist on Linux?
* How to search for the string "my konfi is the best" in files of a directory recursively?
* How to connect to a remote server or what is SSH?
* How to get all environment variables and how can you use them?
* I get "command not found" for ```ifconfig -a```. What can be wrong?
* What happens if I type TAB-TAB?
* What command will show the available disk space on the Unix/Linux system?
* What command is used to lookup DNS records?
* What Unix/Linux commands will alter a files ownership, files permissions?
* What does ```chmod +x FILENAME```do?
* What does the permission 0750 on a file mean?
* What does the permission 0750 on a directory mean?
* How to add a new system user without login permissions?
* How to add/remove a group from a user?
* What is a bash alias?
* How do you set the mail address of the root/a user?
* What does CTRL-c do? What signal does it send.
* What is in /etc/services?
* How to redirect STDOUT and STDERR in bash? (> /dev/null 2>&1)
* What is the difference between UNIX and Linux
* What is the difference between Telnet and SSH?
* Explain the three load averages and what do they indicate

##### [ghavil](https://github.com/jfledvin) additions (filtered to not be too repetitive with above)

* You are adding a brand new hard drive to the second SATA port of a server. Explain how you go about this.
* You have console on a linux box. After running `ifconfig` you only see the loop back network interface. What do you do to get this machine back online? Situation: Physical box in datacenter with cable plugged in.
* You’re trying to run some application, but it keeps failing to start due to an inability to open the necessary port it wants to listen on.  You run ```netstat -an | grep LISTEN | grep <portnum>```, but don’t see anything listening on that port.  What could be going on here?
* You backup your logs and use logrotate to compress and archive all old logs. You need to examine a log, two months old. What would you suggest without decompressing the compressed file?
* How do you see the permissions on a file or directory?
* How would you set the permissions on the file secure.txt so that the owner can read and write but the group and others can’t read, write or execute?
* What is RAID (stand for)/How does RAID work on a basic level? 
* Briefly explain RAID0/1/5/6/10, how much space is usable compared to total, reliability, performance.
* What happens when you telnet to foobar.com on port 80?
* How does a URL translate to an IP?
* Ports that are used for: HTTP(s), DNS, SSH, Telnet, BGP, LDAP, LDAPS, IRC/IRCS, SNMP, IMAP, SMTP 
* What is an ephemeral port? What are they used for?
* Describe the Linux run levels. How would you change the default run level? 


####[[⬆]](#toc) <a name='medium'>Medium Linux Questions:</a>

* What do the following commands do?
 * ```tee```
 * ```awk```
 * ```tr```
 * ```cut```
 * ```tac```
 * ```curl```
 * ```wget```
 * ```watch```
 * ```tail```
* What does a ```&``` after a command do?
* What does ```& disown``` after a command do?
* What is a packet filter and how does it work?
* What is swap and what is it used for?
* What is an A record, an NS record, a PTR record, a CNAME record, an MX record?
 * Are there any other RRs and what are they used for?
* What is the sticky bit?
* What is the difference between hardlinks and symlinks? What happens when you remove the source to a symlink/hardlink?
* What is an inode and what fields are stored in an inode?
* Howto force/trigger a file system check on next reboot?
* What is SNMP and what is it used for?
* What is a runlevel and how to get the current runlevel?
* What is SSH port forwarding?
* What is the difference between local and remote port forwarding?
* What steps to add a user to a system without using useradd/adduser?
* What is MAJOR and MINOR numbers of special files?
* Describe a scenario when you get a "filesystem is full" error, but 'df' shows there is free space.
* Describe a scenario when deleting a file, but 'df' not showing the space being freed.
* Describe how 'ps' works.
* What happens to a child process that dies and has no parent process to wait for it and what’s bad about this?
* How to know which process listens on a specific port?

##### [ghavil](https://github.com/jfledvin) additions (filtered to not be too repetitive with above)

* What does kill do?
* What are the different Linux boot levels?
* How would you remove all ```*.pyc``` files from a directory, recursively?
* You're cleaning up your computer and have a junk drop folder…full of tons of various files. How would you grab only the files modified within the last 15 days?
* Describe (don't need exact commands/lines) how you'd configure a white-list iptables setup in front of an FTP server. Hint: there are two answers.
* How do you change how often a file system check is run at boot time? 
* What are the steps to add a user to a system without using useradd/adduser?
* How would you send a test email via command line?
* What 'masquerade' means in context of iptables
* What would the output of the following look like?
```"date; ps aux | awk `{print $1}' | sort | uniq | wc -l" >> output.log```
* So after fixing an out of control application earlier in the day, you notice that your server’s partition is filling up.  After poking around you see that the angry application from earlier has naturally flooded its log for today with error messages, which has almost filled the partition.  Hurray, more cleanup!  You check your log aggregation system (Splunk/Logstash/whatever) and confirm that all logs are up to date, so you wipe out today’s log with an rm.  You come back 10 minutes later and notice that, while the log file is gone, disk space hasn’t recovered!  What’s going on here?


####[[⬆]](#toc) <a name='hard'>Hard Linux Questions:</a>

* What is the difference between processes and threads?
* What is a tunnel and how you can bypass a http proxy?
* What is the difference between IDS and IPS?
* What shortcuts do you use on a regular basis?
* What is the Linux Standard Base?
* What is an atomic operation?
* Your freshly configured http server is not running after a restart, what can you do?
* What kind of keys are in ~/.ssh/authorized_keys and what it is this file used for?
* I've added my public ssh key into authorized_keys but I'm still getting a password prompt, what can be wrong?
* Did you ever create RPM's, DEB's or solaris pkg's?
* What does ```:(){ :|:& };:``` do on your system and why you would care about that?
* How trace system call and signal?
* What's happening when the Linux kernel is starting the OOM killer, how does it choose which process to kill first.
* Describe the linux boot process with as much detail as possible, starting from when the system is powered on and ending when you get a prompt.
* What's a chroot jail?
* When trying to umount a directory it says it's busy, how to find out which PID holds the directory?
* What's LD_PRELOAD and when it's used?
* You run a binary and nothing happens, how do you debug what's doing?

##### [ghavil](https://github.com/jfledvin) additions (filtered to not be too repetitive with above)

* What is PID 0?
* On a RHEL/Centos 6.5 box, how would you configure rsyncd to run as a service and listen on a specific port of your choosing?


####[[⬆]](#toc) <a name='expert'>Expert Linux Questions:</a>

* A running process gets ```EAGAIN: Resource temporarily unavailable``` on reading a socket. How you can close this bad socket/file descriptor without killing the process?


####[[⬆]](#toc) <a name='network'>Networking Questions:</a>

* What is localhost and why would ```ping localhost``` fail?
* What is the similarity between "ping" & "traceroute" ? How is traceroute able to find the hops.
* What command is used to show all open ports and/or socket connections on a machine?
* Is 300.168.0.123 a valid IPv4 address?
* Which IP ranges/subnets are "private" or "non-routable" (RFC 1918)?
* What is a VLAN?
* What is ARP and what is it used for?
* What is the difference between TCP and UDP?
* What is the purpose of a default gateway?
* What command is used to show the route table for a machine?
* A TCP connection on a network can be uniquely defined by 4 things. What are those things?
* When a client running a web browser connects to a web server, what is the source port and what is the destination port of the connection?
* How do you add an IPv6 address to a specific interface?
* You have added an IPv4 and IPv6 address to interface eth0. A ping to the v4 address is working but a ping to the v6 address gives yout the response ```sendmsg: operation not permitted```. What could be wrong?

##### [ghavil](https://github.com/jfledvin) additions (filtered to not be too repetitive with above)

* What is the TCP handshake?
* Can you block pings by blocking a What ISO network layer does ICMP run on? 
* Please give me an example of a device that operates primarily at each of the first three layers of the OSI networking model.
* How do you prevent your organization’s users from bypassing your organization’s DNS servers? (I.e. You want to force your users to only use the company DNS servers
* Draw a picture of a network infrastructure that could support blank (maybe a small office of 50 people, maybe a grocery store, etc..).

####[[⬆]](#toc) <a name='web'>Front-end Questions:</a>

* What differences exist between HTTP/1.0 and 1.1
* Define HTTP GET vs. POST requests. Why would you use one over the other?
* What is the difference b/w static and dynamic site content? Examples?
* What is a CDN and what kind of content would it contain?
* Do you know what Cloudflare is? If so, describe in latence terms how their anycast system works to provide the content from the closeest possible location to a client.
* Why might it help to serve content from multiple domains?
* Why would it be advantageous to utilize a jquery link via Google.com on in your source code rather than hosting it yourself?
* How can you monitor or watch the number of connections to a site served via Apache or nginx?
* What is minification and how can it help page load times from a client's browser?
* Explain how a browser gets a webpage from a server. (gets html and builds from there)

####[[⬆]](#toc) <a name='devop'>DevOp Questions:</a>

* Can you describe your workflow when you create a script?
* What is GIT?
* What is a dynamically/statically linked file?
* What does "configure && make && make install"?
* What is puppet/chef/ansible used for?
* How do you create a new mysql user?
* How do you create a new postgres user?
* What is a virtual IP address? What is a cluster?
* How print the strings of printable characters in files?
* How look shared library dependencies?
* What is Automake and Autoconf?
* ./configure shows an error that libfoobar is missing on your system, how could you fix this, what could be wrong?
* Advantages/disadvantages of script vs compiled program.
* What is the difference between fork and thread? And parent and child process in fork system call?
* What's the relationship between continuous delivery and DevOps?
* What are the important aspects of a system of continous integration and deployment?


####[[⬆]](#toc) <a name='fun'>Fun Questions:</a>

* A careless sysadmin executes the following command: ```chmod 444 /bin/chmod ``` - what do you do to fix this?
* I've lost my root password, what can I do?
* I've rebooted a remote server but after 10 minutes I'm still not able to ssh into it, what can be wrong?
* If you were stuck on a desert island with only 5 command-line utilities, which would you choose?
* You come across a random computer and it appears to be a command console for the universe. What is the first thing you type?
* Tell me about a creative way that you've used SSH?


####[[⬆]](#toc) <a name='demo'>Demo Time:</a>

* Unpack test.tar.gz without man pages or google.
* Remove all "*.pyc" files from testdir recursively?
* Search for "my konfu is the best" in all *.py files.
* Replace the occurrence of "my konfu is the best" with "I'm a linux jedi master" in all *.txt files.
* :interrobang: more on files ... cut, tr, awk ...
* Test if port 443 on a machine with IP address X.X.X.X is reachable.
* Get http://myinternal.webserver.local/test.html via telnet.
* How to send an email without a mail client, just on the command line?
* Write a ```get_prim``` method in python/perl/bash/pseudo.
* Find all files which have been accessed within the last 30 days.
* Explain the following command ```(date ; ps -ef | awk ‘{print $1}’ | sort | uniq | wc -l ) >> Activity.log```
* Write a script to list all the differences between two directories.
* Write a program in any language you choose, to reverse a file.
* In a log file with contents as ```<TIME> : [MESSAGE] : [ERROR_NO] - Human readable text``` display summary/count of specific error numbers that occured every hour or a specific hour


####[[⬆]](#toc) <a name='references'>Other Great References:</a>

Some questions are 'borrowed' from other great references like:

* https://github.com/darcyclarke/Front-end-Developer-Interview-Questions
* https://github.com/kylejohnson/linux-sysadmin-interview-questions/blob/master/test.md
* https://github.com/gurmeet1109/docgurmeet/tree/master/InterviewQuestionsSamples
* http://slideshare.net/kavyasri790693/linux-admin-interview-questions
