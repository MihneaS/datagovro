Ansible won't work by default on Windows with Vagrant. A simpler solution is:

1. `vagrant up` and wait for the provisioning step to fail
2. Use putty to log into the machine
3. `sudo apt-get update && sudo apt-get install ansible`
4. Edit `/etc/ansible/hosts` and add `localhost ansible_connection=local` on the last line
5. Run `ansible-playbook /vagrant/provisioning/playbook.yml` in the shell.
