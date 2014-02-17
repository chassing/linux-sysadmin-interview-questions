linux-sysadmin-interview-questions
==================================

A collection of linux sysadmin/devop interview questions. Feel free to contribute via pull requests or email messages.


## <a name='toc'>Table of Contents</a>

  1. [Original Contributors](#contributors)
  1. [General Questions](#simple)
  1. [Simple Linux Questions](#simple)
  1. [Medium Linux Questions](#medium)
  1. [Hard Linux Questions](#hard)
  1. [Networking Questions](#network)
  1. [DevOp Questions](#devop)
  1. [Fun Questions](#fun)
  1. [Demo Time](#demo)
  1. [Other Great References](#references)


####[[⬆]](#toc) <a name='contributors'>Original Contributors:</a>

The majority of the questions were collected from:

* https://github.com/gurmeet1109/docgurmeet/tree/master/InterviewQuestionsSamples
* https://github.com/kylejohnson/linux-sysadmin-interview-questions/blob/master/test.md


####[[⬆]](#toc) <a name='simple'>General Questions:</a>

* What did you learn yesterday/this week?
* Talk about your preferred development/administration environment. (OS, Editor, Browsers, Tools etc.)
* What function does DNS play on a network?
* What is a proxy and how does it work?
* What is HTTP?
* What is SMTP? Give the basic scenario of how a mail message is delivered via SMTP?
* What is RAID? What is RAID0, RAID1, RAID5, RAID10?
* What is a level 0 backup? What is an incremental backup?
* Describe the general file system hierarchy of a Linux system.


####[[⬆]](#toc) <a name='simple'>Simple Linux Questions:</a>

* What is the name and the UID of the administrator user?
* How to list all files, including hidden one, in a directory?
* What is the Unix/Linux command to remove a directory and its contents?
* What command will show you free/used memory? Does free memory exists on linux?
* How to search for the string "my konfi is the best" in files of a directory recursively?
* How to connect to a remote server or what is SSH?
* How to get all environment variables and how can you use them?
* I get "command not found" for ```ifconfig -a```. What can be wrong?
* What happens if I type TAB-TAB?
* What command will show the available disk space on the Unix/Linux system?
* What command is used to lookup DNS records?
* What Unix/Linux commands will alter a file's ownership, file's permissions?
* What does the permission 0750 on a file mean?
* What does the permission 0750 on a directory mean?
* How to add a new system user without login permissions?
* How to add/remove a group from a user?


####[[⬆]](#toc) <a name='medium'>Medium Linux Questions:</a>

* What does the ```tee``` command?
* What does the ```awk``` command?
* What does the ```tr``` command?
* What does the ```cut``` command?
* What does the ```tuc``` command?
* What does a ```&``` after a command do?
* What is a packet filter and how does it work?
* What is swap and what is it used for?
* What is an A record, a NS record, a PTR record, a CNAME record, a MX record?
* What is the sticky bit?
* What is the difference between hardlink and symlink? What happens when you remove the source to a symlink/hardlink?
* Howto force/trigger a file system check on next reboot?


####[[⬆]](#toc) <a name='hard'>Hard Linux Questions:</a>

* What is the difference between processes and threads?
* What is a tunnel and how you can bypass a http proxy?
* What is the difference between IDS and IPS?
* What shortcuts do you use on a regular basis?
* What is the linux standard base?
* What is an atomic operation?
* Your fresh configured http server is not running after a restart, what can you do?
* What kind of keys are in ssh/authorized_keys and what it is used for?
* I've added my public ssh key into authorized_keys but I'm still getting a password prompt, what can be wrong?
* Did you ever create RPM's, DEB's or solaris pkg's?


####[[⬆]](#toc) <a name='network'>Networking Questions:</a>

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
* You have added an IPv4 and IPv6 address to interface eth0. A ping to the v4 address is working but a ping to the v6 address gives yout the response ```sendmg: operation not permitted```. What could be wrong?


####[[⬆]](#toc) <a name='devop'>DevOp Questions:</a>

* Can you describe your workflow when you create a script?
* What is GIT?
* What is a dynamically/statically linked file?
* What is "configure && make && make install"
* What is puppet/chef/ansible used for?
* How do you create a new mysql user?
* How do you create a new postgres user?
* What is a virtual IP address? What is a cluster?


####[[⬆]](#toc) <a name='fun'>Fun Questions:</a>

* A careless sysadmin executes the following command: ```chmod 444 chmod ``` - what do you do to fix this?
* I've lost my root password, what can I do?
* I've rebooted a remote server but after 10 minutes I'm still not able to ssh into it, what can be wrong?


####[[⬆]](#toc) <a name='demo'>Demo Time:</a>

* Unpack test.tar.gz without man pages or google.
* Remove all "*.pyc" files from testdir recursively?
* Search for "my konfu is the best" in all *.py files.
* Replace the occurrence of "my konfu is the best" with "I'm a linux jedi master" in all *.txt files.
* :interrobang: more on files ... cut, tr, awk ...
* Test port 443 on a machine with IP address X.X.X.X is reachable.
* Get http://myinternal.webserver.local/test.html via telnet.
* How to send an email without a mail client, just on the command line?
* Write a get_prim python/perl/bash/pseudo script.


####[[⬆]](#toc) <a name='references'>Other Great References:</a>

Some questions are 'borrowed' from other great references like:

* https://github.com/darcyclarke/Front-end-Developer-Interview-Questions
* https://github.com/kylejohnson/linux-sysadmin-interview-questions/blob/master/test.md
* https://github.com/gurmeet1109/docgurmeet/tree/master/InterviewQuestionsSamples
