# Ansible Playbook for RHEL CoreOS to set hostname from Bastion server

## Usage

1. Update the template file to have the correct ip addresses and fully qualified domain names (FQDN).

    Example:

    ```shell
    [all]
    10.10.10.23 new_hostname=ocp1.example.com
    10.10.10.24 new_hostname=ocp2.example.com
    10.10.10.25 new_hostname=ocp3.example.com
    ```

2. Run the playbook from the bastion server that is keyed to the RHEL CoreOS nodes.

    ```shell
    ansible-playbook playbook.yml -i inventory.txt
    ```