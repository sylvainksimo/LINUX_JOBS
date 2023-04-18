One, Install the OpenSSH server:
      >>sudo apt-get update
      >>sudo apt-get install openssh-server


Two, Verify that the OpenSSH server is running:
      >>sudo systemctl status ssh
  If the OpenSSH server is not running, start it using the following command:
      >>sudo systemctl start ssh


Three, Allow SSH traffic through the firewall:
      >>sudo ufw allow ssh


Four, Configure the SSH server to allow remote login:
      >>sudo nano /etc/ssh/sshd_config
  Look for the line that reads #PermitRootLogin prohibit-password and change it to PermitRootLogin yes.
  Look for the line that reads #PasswordAuthentication yes and change it to PasswordAuthentication yes.
  Save the changes and exit the editor.


Five, Restart the SSH server for the changes to take effect:
      >>sudo systemctl restart ssh

After following these steps, you should be able to connect to your Ubuntu desktop using an SSH client such as PuTTY or OpenSSH.
