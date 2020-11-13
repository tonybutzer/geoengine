# See Makefile

## References

http://www.ntweekly.com/2020/02/16/install-python-3-8-on-amazon-linux-2-ec2-instance/
https://docs.aws.amazon.com/sdk-for-javascript/v2/developer-guide/setting-up-node-on-ec2-instance.html


## nodejs is per user


Procedure

The following procedure helps you install Node.js on an Amazon Linux instance. You can use this server to host a Node.js web application.

To set up Node.js on your Linux instance

    Connect to your Linux instance as ec2-user using SSH.

    Install node version manager (nvm) by typing the following at the command line.

Warning

AWS does not control the following code. Before you run it, be sure to verify its authenticity and integrity. More information about this code can be found in the nvm

GitHub repository.

- curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.34.0/install.sh | bash

We will use nvm to install Node.js because nvm can install multiple versions of Node.js and allow you to switch between them.

Activate nvm by typing the following at the command line.

- . ~/.nvm/nvm.sh

Use nvm to install the latest version of Node.js by typing the following at the command line.

- nvm install node

Installing Node.js also installs the Node Package Manager (npm) so you can install additional modules as needed.

Test that Node.js is installed and running correctly by typing the following at the command line.

- node -e "console.log('Running Node.js ' + process.version)"

This displays the following message that shows the version of Node.js that is running.

Running Node.js VERSION


Note

The node installation only applies to the current EC2 session. Once the EC2 instance goes away, you'll have to re-install node again. The alternative is to make an AMI of the EC2 instance once you have the configuration that you want to keep, as described in the following section.

