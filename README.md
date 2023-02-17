# File_copy
-name: Ansible Copy file from Local to remote
hosts: remoteserver
tasks:
	-name: playbook to copy file
	become: true
	src: /etc/passwd
	dest://tmp/passwd
	owner:apache 
	mode: 0644
