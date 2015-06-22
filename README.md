Linux System Administrator/DevOps Interview Questions
====================================================

A collection of linux sysadmin/devops interview questions. Feel free to contribute via pull requests, issues or email messages.


## <a name='toc'>Table of Contents</a>

  1. [Contributors](#contributors)
  1. [General Questions](#general)
  1. [Simple Linux Questions](#simple)
  1. [Medium Linux Questions](#medium)
  1. [Hard Linux Questions](#hard)
  1. [Expert Linux Questions](#expert)
  1. [Networking Questions](#network)
  1. [MySQL Questions](#mysql)
  1. [DevOps Questions](#devop)
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
* [pedroguima](https://github.com/pedroguima)
* Ben


####[[⬆]](#toc) <a name='general'>General Questions:</a>

* What did you learn yesterday/this week?
* Talk about your preferred development/administration environment. (OS, Editor, Browsers, Tools etc.)
* Tell me about the last major Linux project you finished.
* Tell me about the biggest mistake you've made in [some recent time period] and how you would do it differently today. What did you learn from this experience?
* Why we must choose you?
* What function does DNS play on a network?
* What is HTTP? 
* What is an HTTP proxy and how does it work?
* Describe briefly how HTTPS works.
* What is SMTP? Give the basic scenario of how a mail message is delivered via SMTP.
* What is RAID? What is RAID0, RAID1, RAID5, RAID10?
* What is a level 0 backup? What is an incremental backup?
* Describe the general file system hierarchy of a Linux system.


####[[⬆]](#toc) <a name='simple'>Simple Linux Questions:</a>

* What is the name and the UID of the administrator user? Answer:`0`
* How to list all files, including hidden one, in a directory? Answer:`ls -la`
* What is the Unix/Linux command to remove a directory and its contents? Answer:`rm -rf <directory_name>`
* Which command will show you free/used memory? Does free memory exist on Linux? Answer:`htop` or `top` or `vmstat`
* How to search for the string "my konfi is the best" in files of a directory recursively? Answer:`grep -r "my konfi is the best" <directory_name>`
* How to connect to a remote server or what is SSH? Answer:`ssh <username>@<host_ip>` [more](http://www.differencebetween.net/technology/internet/difference-between-telnet-and-ssh/)
* How to get all environment variables and how can you use them? Answer:`env` using them `echo $PATH` 
* I get "command not found" when I run ```ifconfig -a```. What can be wrong? Answer:`/sbin` is not part of `PATH` environment variable, do `export PATH=$PATH:/sbin`
* What happens if I type TAB-TAB? Answer:Would show `Display all 1234 possiblilities (y/n)`
* What command will show the available disk space on the Unix/Linux system? Answer:`df -h`
* What commands do you know that can be used to check DNS records?Answer: `nslookup -type=A google.com`
* What Unix/Linux commands will alter a files ownership, files permissions? Answer:`chmod`
* What does ```chmod +x FILENAME```do? Answer: sets execute permission on the file.
* What does the permission 0750 on a file mean? [Answer](http://meinit.nl/linux-permission-system-explained)
* What does the permission 0750 on a directory mean? [Answer](http://meinit.nl/linux-permission-system-explained)
* How to add a new system user without login permissions? [Answer](http://superuser.com/questions/77617/how-can-i-create-a-non-login-user)
* How to add/remove a group from a user? [Answer](http://www.cyberciti.biz/faq/howto-linux-add-user-to-group/)
* What is a bash alias? Answer: `alias ll="ls -l"` this will execute `ls -l` on the prompt when we execute `ll`
* How do you set the mail address of the root/a user? [Answer](http://unix.stackexchange.com/a/26670)
* What does CTRL-c do? Answer: sends `SIGINT` and CTRL-z sends `SIGTSTP` [more](http://askubuntu.com/a/510816)  
* What is in /etc/services? Answer: Server to Port Translation. [more](https://access.redhat.com/articles/1761)
* How to redirect STDOUT and STDERR in bash? Answer: `(> /dev/null 2>&1)` 
* What is the difference between UNIX and Linux. Answer: UNIX commercial proprietary OS, Linux is Free and Opensourve [more](http://www.golinuxhub.com/2014/04/what-is-differencecomparison-between.html) 
* What is the difference between Telnet and SSH? Answer: Both network Communication protocol, telnet unsecure (plain-text), ssh is secure shell. [more](http://www.differencebetween.net/technology/internet/difference-between-telnet-and-ssh/)
* Explain the three load averages and what do they indicate. [Answer](http://blog.scoutapp.com/articles/2009/07/31/understanding-load-averages)



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
* What does a ```&``` after a command do? Runs the command in background. 
* What does ```& disown``` after a command do? 
* What is a packet filter and how does it work?
* What is Virtual Memory? 
* What is swap and what is it used for? 
* What is an A record, an NS record, a PTR record, a CNAME record, an MX record?
* Are there any other RRs and what are they used for?
* What is a Split-Horizon DNS?
* What is the sticky bit?
* What does the immutable bit to a file?
* What is the difference between hardlinks and symlinks? What happens when you remove the source to a symlink/hardlink?
* What is an inode and what fields are stored in an inode?
* Howto force/trigger a file system check on next reboot?
* What is SNMP and what is it used for?
* What is a runlevel and how to get the current runlevel?
* What is SSH port forwarding?
* What is the difference between local and remote port forwarding?
* What are the steps to add a user to a system without using useradd/adduser?
* What is MAJOR and MINOR numbers of special files?
* Describe a scenario when you get a "filesystem is full" error, but 'df' shows there is free space.
* Describe a scenario when deleting a file, but 'df' not showing the space being freed.
* Describe how 'ps' works.
* What happens to a child process that dies and has no parent process to wait for it and what’s bad about this?
* Explain briefly each one of the process states.
* How to know which process listens on a specific port?
* You run a bash script and you want to see its output on your terminal and save it to a file at the same time. How could you do it?
* Explain what echo "1" > /proc/sys/net/ipv4/ip_forward does.
* Describe briefly the steps you need to take in order to create and install a valid certificate for the site https://foo.example.com.
* Can you have several HTTPS virtual hosts sharing the same IP?
* What is a wildcard certificate?
* Which Linux file types to you know?
* What is the difference between a process and a thread? And parent and child processes after a fork system call?
* What is the difference between exec and fork?
* What is "nohup" used for?
* What is the difference between these two commands?
 * ```myvar=hello```
 * ```export myvar=hello```
* How many NTP servers would you configure in your local ntp.conf?
* What does the column 'reach' mean in ```ntpq -p``` output?


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
* What does ```:(){ :|:& };:``` do on your system?
* How do you catch a Linux signal on a script?
* Can you catch a SIGKILL?
* What's happening when the Linux kernel is starting the OOM killer and how does it choose which process to kill first?
* Describe the linux boot process with as much detail as possible, starting from when the system is powered on and ending when you get a prompt.
* What's a chroot jail?
* When trying to umount a directory it says it's busy, how to find out which PID holds the directory?
* What's LD_PRELOAD and when it's used?
* You ran a binary and nothing happened. How would you debug this?
* What are cgroups? Can you specify a scenario where you could use them?


####[[⬆]](#toc) <a name='expert'>Expert Linux Questions:</a>

* A running process gets ```EAGAIN: Resource temporarily unavailable``` on reading a socket. How can you close this bad socket/file descriptor without killing the process?


####[[⬆]](#toc) <a name='network'>Networking Questions:</a>

* What is localhost and why would ```ping localhost``` fail?
* What is the similarity between "ping" & "traceroute" ? How is traceroute able to find the hops.
* What is the command used to show all open ports and/or socket connections on a machine?
* Is 300.168.0.123 a valid IPv4 address?
* Which IP ranges/subnets are "private" or "non-routable" (RFC 1918)?
* What is a VLAN?
* What is ARP and what is it used for?
* What is the difference between TCP and UDP?
* What is the purpose of a default gateway?
* What is command used to show the routing table on a Linux box?
* A TCP connection on a network can be uniquely defined by 4 things. What are those things?
* When a client running a web browser connects to a web server, what is the source port and what is the destination port of the connection?
* How do you add an IPv6 address to a specific interface?
* You have added an IPv4 and IPv6 address to interface eth0. A ping to the v4 address is working but a ping to the v6 address gives yout the response ```sendmsg: operation not permitted```. What could be wrong?
* What is SNAT and when should be used?
* Explain how could you ssh login into a Linux system that DROPs all new incomming packets using a SSH tunnel.
* How do you stop a DDoS?


####[[⬆]](#toc) <a name='mysql'>MySQL questions:</a>

* How do you create a user?
* How do you provide privileges to a user?
* What is the difference between a "left" and a "right" join?
* Explain briefly the differences between InnoDB and MyISAM.
* Describe briefly the steps you need to follow in order to create a simple master/slave cluster.
* Why should you run "mysql_secure_installation" after installing MySQL?
* How do you check which jobs are running?


####[[⬆]](#toc) <a name='devop'>DevOps Questions:</a>

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
* What's the relationship between continuous delivery and DevOps?
* What are the important aspects of a system of continous integration and deployment?


####[[⬆]](#toc) <a name='fun'>Fun Questions:</a>

* A careless sysadmin executes the following command: ```chmod 444 /bin/chmod ``` - what do you do to fix this? `busybox chmod +x /bin/chmod`
* I've lost my root password, what can I do? Answer: Login as single user mode and recover the password. 
* I've rebooted a remote server but after 10 minutes I'm still not able to ssh into it, what can be wrong?
* If you were stuck on a desert island with only 5 command-line utilities, which would you choose?
* You come across a random computer and it appears to be a command console for the universe. What is the first thing you type? `pwd` 
* Tell me about a creative way that you've used SSH? 
* You have deleted by error a running script, what could you do to restore it? 


####[[⬆]](#toc) <a name='demo'>Demo Time:</a>

* Unpack test.tar.gz without man pages or google. `tar -xvzf test.tar.gz`
* Remove all "*.pyc" files from testdir recursively? `find . -name "*.pyc" -exec rm -rf {} +`
* Search for "my konfu is the best" in all *.py files. `grep --color -r "my konfu is the best" *.py`
* Replace the occurrence of "my konfu is the best" with "I'm a linux jedi master" in all *.txt files. `find . -name "*.py" -exec sed -i 's/my\ konfu\ is\ the\ best/I'm\ a\ linux\ jedi\ master/g' {} +`
* Test if port 443 on a machine with IP address X.X.X.X is reachable. `telnet X.X.X.X 443`
* Get http://myinternal.webserver.local/test.html via telnet. 

    step 1: `telnet myinternal.webserver.local 80` <enter>
    step 2: `GET /test.html HTTP/1.1` <enter>

* How to send an email without a mail client, just on the command line? `echo "This is my Mail" | mailx -v -A gmail_account_in_mailrc -s "This is my Subject" ahmed@mail.com`
* Write a ```get_prim``` method in python/perl/bash/pseudo. `SEE END OF README`
* Find all files which have been accessed within the last 30 days. `find <src_directory> -mmin 43200` (43200 minutes).  
* Explain the following command ```(date ; ps -ef | awk ‘{print $1}’ | sort | uniq | wc -l ) >> Activity.log``` - Number if different users running the server.
* Write a script to list all the differences between two directories.
* In a log file with contents as ```<TIME> : [MESSAGE] : [ERROR_NO] - Human readable text``` display summary/count of specific error numbers that occured every hour or a specific hour. ```for item in ERRORCODE1 ERRORCODE2 ERRORCODE3 ERRORCODE4; do echo ERROR CODE $item : `find <src_dir> -cmin -60 -exec grep $item {} + | wc -l`;  done```




####[[⬆]](#toc) <a name='references'>Other Great References:</a>

Some questions are 'borrowed' from other great references like:

* https://github.com/darcyclarke/Front-end-Developer-Interview-Questions
* https://github.com/kylejohnson/linux-sysadmin-interview-questions/blob/master/test.md
* https://github.com/gurmeet1109/docgurmeet/tree/master/InterviewQuestionsSamples
* http://slideshare.net/kavyasri790693/linux-admin-interview-questions
* https://github.com/gurmeet1109/docgurmeet/tree/master/InterviewQuestionsSamples
* https://github.com/kylejohnson/linux-sysadmin-interview-questions/blob/master/test.md


### `get_prime` function in python.

    def get_prime(num):
        print num
    
        if num <= 1:
            print "Not a Prime Number"
        else:
            for i in range(2, num):
                if num%i == 0:
                    print num, "is Not Prime"
                    print i, "x", num//i, "=", num
                    break
            else:
                print "Prime"
    
    get_prime(int(input("Enter a Number:")))