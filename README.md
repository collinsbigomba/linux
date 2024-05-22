# linux

## configuring ssh port 22
This enables users to remotly login from any machine that also has ssh on it or putty inorder to access the server 
  - First install ssh on the server if its not installed
  <br><img src="https://github.com/collinsbigomba/linux/blob/main/images/ssh1.png" /> </br>
  -Start the ssh service with the command as follows
  <br><img src="https://github.com/collinsbigomba/linux/blob/main/images/ssh2.png" /> </br>
  - configure its configuration file (/etc/ssh/sshd.conf) inorder to make the connection successfull
   <br><img src="https://github.com/collinsbigomba/linux/blob/main/images/ssh3.png" /> </br>
    # Add some parameters to improve the security of your server
   - PermitRootLogin no 
   - passwordAuthentication no 
   - change your ssh port number to a different one 
   - pubkeyAuthentication yes inorder to enable key based authentication on your server 
    <br><img src="https://github.com/collinsbigomba/linux/blob/main/images/ssh.png" /> </br>

  - Generate the keys with the following command
    <br><img src="https://github.com/collinsbigomba/linux/blob/main/images/keygen1.png" /> </br>
  - Copy the public key to your server
   <br><img src="https://github.com/collinsbigomba/linux/blob/main/images/copy.png" /> </br>
  - start a basg shell with the following command
   <br><img src="https://github.com/collinsbigomba/linux/blob/main/images/bash.png" /> </br>
  - Add the private key in memory such that you wont be typing your password for every login but rather until the session is ended
   <br><img src="https://github.com/collinsbigomba/linux/blob/main/images/add.png" /> </br>
  - Start ssh with the command as follows
  - ssh -p 22 192.168.2.3


  
