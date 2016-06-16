Ansible Reachability Test
=========================
Sample ansible playbook to install nmap and test host/port reachability between machines. 
The problem is default user name is different for Amazon/Redhat (ec2-user) and Ubuntu (ubuntu) in AWS.
Tha playbook considers different types of OS's (including windows)

Installation
------------

    1. Export AWS variables  AWS_SECRET_ACCESS_KEY, AWS_ACCESS_KEY_ID
    2. ssh-agent bash
    3. ssh-add ~/.ssh/aws.pem
    4. ansible-vault create group_vars/ami_29eb7e5a.yml
    5. Set contents from sample_win_group
    6. Launch windows instances with winrm enabled (see win_userdata example)

Usage
-----

    ansible-playbook -i ec2.py play1.yml  --ask-vault-pass  from folder ami_based_play




