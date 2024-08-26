# Step-by-Step-Guide-to-Creating-a-CentOS-VM-with-Vagrant

Step-by-Step Guide to Creating a CentOS VM with Vagrant
As a data engineer on the path to becoming a Cloud Engineer, I'm excited to share my journey with you. This project marks the beginning of my transition into the world of Cloud computing.
On this project, I will be setting up a CentOS 9 operating system on a Vagrant-managed virtual machine. By leveraging Vagrant, I will automate the creation and configuration of the CentOS environment.
Tools Used
Vagrant: A tool for automating the creation and management of virtual environments.
CentOS: A free, enterprise-class Linux distribution, ideal for server environments.
Git Bash: A command-line tool that allows users to run Git commands and other Unix-based utilities on Windows.

CentOS VM Setup Breakdown
Create a Vagrant Directory:

Navigate to the C: drive on your PC.
Use the command mkdir vagrant-vms to create a directory named vagrant-vms.
Verify the directory creation.
cd vagrant-vms : to change to the newly created vagrant directory.
pwd: to confirm the present working directory.

2. Set Up the CentOS Directory:
Within the Vagrant directory, create a subdirectory named CentOS using the mkdir centos command.
This directory will contain all files related to the CentOS virtual machine.

3. Prepare the Vagrantfile:
We will place a Vagrantfile in the CentOS directory to define the VM configuration.

4. Obtain the Vagrant Box Name:
Visit the Vagrant Cloud and search for CentOS 9
For this project, we will use the box eurolinux-vagrant/centos-stream-9.

5. Initialize the Vagrant Environment:
Copy the box name (eurolinux-vagrant/centos-stream-9).

Open your CLI, navigate to the CentOS directory, and run the following command to initialize the Vagrant environment: vagrant init eurolinux-vagrant/centos-stream-9
Confirm that the initialization was successful by checking for the creation of the Vagrantfile in your directory, using the ls command.

6. Start the Vagrant VM:
Use the vagrant upcommand to start the VM
Vagrant will download the specified box from Vagrant Cloud, store it locally, and create the virtual machine.

7. Verify the Box and VM Status:
To view the list of available boxes on your local machine, run vagrant box list

To check the status of the VM, run vagrant status

8. Access the VM:
Log in to the VM using the vagrant ssh command.
