# ansible_three_tier Application
This repository contains the Ansible playbooks and roles for deploying the three tier application with application server, web server and database server.
# setup
1. **Installing Ansible in the Control node**
      pip install ansible
2. **Configuring the SSH Authentication**
       Ensure passwordless SSH authentication is set up between your Ansible control machine and the remote servers.
# Directory structure
- ansible_three_tier/
    - ansible.cfg : Ansible default configuration settings.
    - inventory.ini : Inventory file defining server groups.
    - playbook.yml : Main Ansible playbook for deploying the application.
    - rools/ : contains Ansible roles for each server type
           - Webserver/ : Role for configuring the webserver
                - tasks/
                     - main.yml
           - Appserver/ : Role for configuring the application server
                - tasks/
                      - main.yml
           - Dbserver/ :Role for configuring the databse server
                 - tasks/
                      - main.yml
