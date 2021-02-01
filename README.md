# midpoint-ansible
Used to automate the midpoint build process using ansible

The playbook contains three variables which you will need to define.
- host: (name or IP of the remote server)
- ansible_default_ipv4.address: IP address of the server, this will be added to /etc/hosts
- ansible_fqdn: Name of the remote server, this will be added to /etc/hosts

Example:

sudo ansible-playbook midpoint.yml --ask-pass -e "host=192.168.1.50 ansible_default_ipv4.address=192.168.1.50 ansible_fqdn=midpointdev"



If you are not familiar with Ansible, start here: https://www.ansible.com/resources/get-started
