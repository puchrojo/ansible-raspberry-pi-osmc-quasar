# ansible-raspberry-pi-osmc-quasar
Install a osmc mit quasar plugin on a raspberry pi 3 mit ansible

Requeriments
* A Linux Computer
* SDD Card
* Raspberry Pi (3)

# Configure
Edit hosts and group_vars/all (Please check DEV_SDD or you could lost your disk content)

Run / Install
# Firs on localhost:
ansible-playbook --ask-become-pass 1-Install-OSMC-on-SDCARD-localhost

# Connect the SDCARD on Raspberry Pi and bootet it:
ansible-playbook 2-Configure-Raspberry-Pi.yml
