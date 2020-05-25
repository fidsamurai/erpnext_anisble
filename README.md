# erpnext_anisble
ansible script to install erpnext
Clone the repo to your system.
Change the following:-
1. inv file with the host/s IPs for the machines that this will deploy too.
2. Inside the group_vars folder there is a file called all change the variables to suit your requirements.

To run the playbook ensure ssh accessiblity from the machines that are going to be used for the setup.
Clone the repo to any directory.
cd into the clone directory.

ansible-playbook -i inv erp-setup.yml -u <username for target server/s> -k -K

There will be 2 prompts, the first for the ssh password the second for sudo(no need to put anything here as it defaults to the ssh password)
