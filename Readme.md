** Make sure to pip install ansible, apt has an older copy **

# Instructions
* Start with a fresh installation of Kali Linux, this is made specifically for an installation using Gnome as it imports some of my keybindings using dconf. If not using Gnome, comment out the line including gnome-shell.yml in `roles/customize-terminal/tasks/main.yml`.
* Install Ansible (pip3 install ansible)
* Clone and enter the repo (git clone)
* ansible-galaxy install -r requirements.yml
* Make sure we have a sudo token (sudo whoami)
* ansible-playbook main.yml

# Off-Video Changes
* Mate-Terminal Colors, I show how to configure it here (https://www.youtube.com/watch?v=2y68gluYTcc). I just did the steps in that video on my old VM to backup the color scheme, then copied it to this repo.
* Evil-Winrm/Certipy/SharpCollection/CME/Impacket, will make a video for these soon
* Updated BurpSuite Activation. Later versions of ansible would hang if a shell script started a process that didn't die. Put a timeout on the java process
