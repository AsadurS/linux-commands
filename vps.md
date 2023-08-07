##Initial Login
The very first step to start using a server is to log in to it. A web server is just like a computer on the web. We cannot connect a physical keyboard and mouse to it. So how do we use it?  We will use an SSH Client to get access to the server's terminal (this remote computer), and once we have access to the terminal, we can start executing commands on this server. 

To log in to our server, we need to know its public IP address, just like you need to know the address of a place before visiting it. 

###Execute the following command on the PowerShell or terminal
  ssh root@your_server_ip

###Creating a non-root user
We will now create a non-root user account that will have restricted access to the machine. This is ideal if you want to have people working for you on the server without doing everything on the server.

##Execute the following command:
  adduser Muhammad
You will be asked to enter some information and a password. Choose a strong password to avoid getting hacked!

We have successfully created an account with basic access. We want this user to be able to elevate to root access when required. This will be useful when you want to use your server and sometimes do something which requires root access.

This will save you the time to log out and log back in as the root user.

###Execute the following command on the server:

usermod -aG sudo muhammad
###You can type the following command to elevate to the root access as and when required.
  sudo su
