
### ADD and  DELETE a user on Linux system and GRANT SUDO privilege ###

sudo adduser username -
	 This root command will create a new user after providing proper root or sudo privilege.

su username -
	
	# This command will ask for user's credentials to login and access its home directory.

id -
	
	# This command will give details groups permission of a logged in user.

groups -     
	
	# This command will show in which groups the current user belongs to.

sudo groups -
	
	# This root command will show if it is under any root privilege or only on its own group.

sudo adduser username sudo - 
	
	# This command will grant sudo (almost root)  privilege to the specified user. The user must logout to get access.

sudo deluser --remove-home -f username -
	
	# This root command will force(-f) to delete the user with its home directory.You must logout that user to delete it.

sudo visudo -
	
	# This root command will take you to write or change users sudo privilege. 
	# Yes, the file /etc/sudoers is intentionally set read-only, even for root! 

Defaults rootpw -
	
	# This line under /etc/sudoers will ask user to enter root password even the user is a sudo user.

passwd user -
	
	# This command will allow user to change its password.

sudo pkill -KILL -u username -
	
	# This root command will logout a user.

last || lastb || last tty || last username -
	
	# This command will show last login session of users with date and time of login.

who || w -
	
	# This command will show who are logged in using terminal.

mail -

	# This command will show your emails.

cat /var/mail/username -
	
	# This command will show you last email.

less +G /var/spool/mail/root -
	
	# This command will show you latest emails.

cp --copy-contents sourcefile destinationfile -

	# This command will copy exact contents of the sourcefile to its destinationfile.

pwd - 

	#This command will print working directory.

tocuh myfile.txt - 

	#This command will create a new text file.

cat myfile.txt -

	#This command will reads files.

mkdir magicdir -
		
	#This command will create a directory.

mv myfile.txt magicdir/ -

	#This command moves a file to a target directory.

rmdir magicdir -

	#This command will give an error if any file resides under magic directory.

rm -r magicdir/ 

	#This command will remove item recursively including the directory.

cmd+r -

	#This command will help you reverse history search of your written commands.

cmd+r -

	#This command typing again will help you to see all sorts of shell command you are searching.

ln -s sysadmin.txt linkSysadmin -
	
	#This command will create soft link for shortcut of the original file.

head sysadmin.txt -

	#This command will present you first 10 lines of a file.

tail sysadmin.txt -

	#This command  will present you last 10 lines of a file.

tail -f /var/log/dmesg -

	#Ths command will tail message log.

shutdown -h -r now +60 -

	#This ia a common shutdown account.

w -

	#This command will give you which users are logged in with what ip address and some more details.New terminal counts as new user.

top -

	#This gives you detials of your process id with top resource hog.

netstat -tupln -
	
	#(tcp, udp, program, listening port, numeric order.

htop -

	#THis command is a utility program to kill,search different kind of process.

## Creating a github account along with git repository for project file push and pull.

# Create a github account.
# Make a repository on github account name it after the project name you are wokring on it.

git init
	# This command will initailized current working directory for git repository update.

echo "#Add some random line" >> README.md

	# This command will add  a line to README.md

git add .

	# This command will add all the files that has been modified on git configuration file.

git commit -m "My first git commit"

	# This command will commit any modified file for git update.

git remote add origin https://github.com/8321/magicdir.git

	# This command will set git url for repository update.

git push -u origin master

	# This command will ask user for account and password for repository update.

git remote set-url origin https://github.com/8321/test.git
git remote -v

	# These command will set url and verify if the repository link is set mistakenly to a non existing repository.
 
	
	

