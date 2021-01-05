Ansible Assignment

task:
	1)ansible for weekly system reboot
	  a) run preboot tasks, use "yum" for upgrades
		b) use "command" module to "reboot" server
		c) run "wait_for" module to wait for 300 seconds 
		   for port 22 to become available before resuming the playbook.
		   the port number can be changed if its not open-ssh
		d) resume playbook on response from port 22
	
	2)Security Guidelines for Server in Ansible
		a) Create playbook boilerplate, YAML file.
		b) Change the password for user account,
		   Create and configure a deploy user account,
		   Configure Public Key Authentication for the deploy Account.
		c) Add deploy user to sudoers, run updates and upgrades.
		d) use "ufw" for iptables configuration, allow only "ssh" traffic.
		e) configure "postfix" to relay daily summary email with "debconf" module.
    f) customize the ssh_port variable, disable ssh for root account.
    
  3)Ansible Rollback
    a) Install ansistrano.rollback using the requirements.yml , add an entry inside it
    b) install the role on the local terminal using ansible-galaxy
    c) create the rollback playbook, add the rollback role inside
    d) from the deploy yml file copy parameters required into the rollback file
    e) now use ansible playbook for rollback mechanism to be applied

      
