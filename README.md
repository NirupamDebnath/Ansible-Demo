# Ansible-Demo

Testbed :
1. Create a vertual machine in virtual box. fedora with2 vpu 2 GB ram wroked well
2. Create the VM with bridged network so that they can connect with each other
3. Clone the created jump vm with option "Create new mac address" and "linked clone to save space"


Installation:
1. sudo dnf install ansible
2. use Remote - SSH to directly work on vm folder over ssh

Commands:
1. ansible target1 -m ping -i inventory.txt
2. ansible target2 -m ping -i inventory.txt
3. ansible all -m ping -i inventory.txt
4. ansible-playbook pingtest-playbook.yaml -i inventory.txt
5. ansible-playbook shutdown-playbook.yaml -i inventory.txt -K