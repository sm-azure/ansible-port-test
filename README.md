# Port Reachability Test Using Ansible
Sample ansible playbook to install nmap and test host/port reachability between machines. 
The problem is default user name is different for Amazon/Redhat (ec2-user) and Ubuntu (ubuntu) in AWS.
Tha playbook considers different types of OS's.

Usage: ansible-playbook -i ec2.py play1.yml from folder ami_based_play
Usage: ansible-playbook port-playbook.yml -i sample_hosts


