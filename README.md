# Ansible Playbook for RHEL CoreOS to set hostname from Bastion server

## Usage

1. Update the template file to have the correct ip addresses and fully qualified domain names (FQDN)
2. Run the playbook from the bastion server that is keyed to the RHEL CoreOS nodes.
    ```shell
    ansible-playbook playbook.yml -i inventory.txt
    ```