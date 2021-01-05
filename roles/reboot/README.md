Reboot
=========
		a) run preboot tasks, use "yum" for upgrades
		b) use "command" module to "reboot" server
		c) run "wait_for" module to wait for 300 seconds 
		   for port 22 to become available before resuming the playbook.
		   the port number can be changed if its not open-ssh
		d) resume playbook on response from port 22
	


Requirements
------------
target machines should be of linux flavour with yum as repository

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: amazon-linux-group
      roles:
         - reboot

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
