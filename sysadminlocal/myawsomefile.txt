
### ADD and  DELETE a user on Linux system and GRANT SUDO privilege

sudo adduser username 
# This root command will create a new user after providing proper root or sudo privilege.

su username 
# This command will ask for user's credentials to login and access its home directory.

id
# This command will give details groups permission of a logged in user.

groups      
# This command will show in which groups the current user belongs to.

sudo groups
# This root command will show if it is under any root privilege or only on its own group.

sudo adduser username sudo 
# This command will grant sudo (almost root)  privilege to the specified user. The user must logout to get access.

sudo deluser --remove-home -f username 
# This root command will force(-f) to delete the user with its home directory.You must logout that user to delete it.

sudo visudo
# This root command will take you to write or change users sudo privilege. 
# Yes, the file /etc/sudoers is intentionally set read-only, even for root!
# The explanation usually offered is that it was set up this way to ensure that admins only ever edit it via the command visudo. 
# However, this theory doesn't quite hold water. 
# Being mode 0440 does nothing to impede sudo nano /etc/sudoers - most text editors will let you edit the file without complaining 
# about the read-only bit. 
# Besides, any time you do mangle /etc/sudoers, the fix may be as simple as su -c visudo, 
# which is nothing compared to the kind of recovery procedure you'd have to go through 
# if you broke something like /etc/inittab (mode 0644). So if there's a good reason for the unorthodox permissions, 
# it's a mystery - contributions welcome. 


Defaults   rootpw
# This line under /etc/sudoers will ask user to enter root password even the user is a sudo user.

passwd user
# This command will allow user to change its password.

sudo pkill -KILL -u username
# This root command will logout a user.

last || lastb || last tty || last username
# This command will show last login session of users with date and time of login.

who || w
# This command will show who are logged in using terminal.

mail
# This command will show your emails.

cat /var/mail/username
# This command will show you last email.

less +G /var/spool/mail/root
# This command will show you latest emails.



001. pwd - print working directory
002. cd ..
003. ls 
004. ls -a
005. tocuh myfile.txt (creates a new text file)
006. gedit myfile.txt (will open myfile in gnome text editor)
007. cat myfile.txt (reads files)
008. mkdir magicdir (makes directory)
009. mv myfile.txt magicdir/ (moves target thing to destination folder)
010. mkdir testrm
011. touch testrm/testfile
012. rmdir testrm will give u an error
013. rm -r testrm/ (will remove item recursively)
014. command or ctrl+a will take you beginning of the line
015. command or ctrl+e will take you end of the line
016. # to comment out during the command line
017. command or ctrl+r will give you for reverse history search
018. command or ctrl+r again to see all sorts of shell command you are searching.
019. touch file3
020. ln -s file3 file3Link
021. nano file3Link
022. head magicfile.txt will present you first 10 line
023. tail mahicfile.txt will present you last 10 line
024. tail -f /var/log/dmesg
025. shutdown -h -r now +60
026. poweroff
027. init 0
028. init 6
029. w (gives you which users are logged in with what ip address and some more details.New terminal counts as new user)
030. top (gives you detials of your process id with top resource hog)
031. netstat -tupln (tcp, udp, program, listening port, numeric order)
032. htop is a utility program to kill,search different kind of process.
033. 
034.
035.


