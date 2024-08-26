# Step-by-Step-Guide-to-Creating-a-CentOS-VM-with-Vagrant

As a data engineer on the path to becoming a Cloud Engineer, I'm excited to share my journey with you. This project marks the beginning of my transition into the world of Cloud computing.

In this project, I will set up a CentOS 9 operating system on a Vagrant-managed virtual machine. By leveraging Vagrant, I will automate the creation and configuration of the CentOS environment.


**Tools Used**

- **Vagrant:** A tool for automating the creation and management of virtual environments.
- **CentOS:** A free, enterprise-class Linux distribution, ideal for server environments.
- **Git Bash:** A command-line tool that allows users to run Git commands and other Unix-based utilities on Windows.


**CentOS VM Setup Breakdown**

**1. Create a Vagrant Directory:**
- Navigate to the **C:** drive on your PC.
- Use the command **mkdir vagrant-vms** to create a directory named **vagrant-vms**.
- Verify the directory creation.
  - **cd vagrant-vms :** to change to the newly created vagrant directory.
  - **pwd:** to confirm the present working directory.

  ![image](https://github.com/user-attachments/assets/1d23a67c-8cca-4daa-bc4d-002e17605edd)


**2. Set Up the CentOS Directory:**
- Within the Vagrant directory, create a subdirectory named **CentOS** using the **mkdir centos** command.
- This directory will contain all files related to the CentOS virtual machine.

  ![image](https://github.com/user-attachments/assets/9a402a67-2911-47e3-8c03-f10c712ee4f4)


**3. Prepare the Vagrantfile:**
  We will place a **Vagrantfile** in the **CentOS** directory to define the VM configuration.

**4. Obtain the Vagrant Box Name:**
- Visit the [Vagrant Cloud](https://portal.cloud.hashicorp.com/vagrant/discover) and search for CentOS 9
- For this project, we will use the box **eurolinux-vagrant/centos-stream-9.**

  ![image](https://github.com/user-attachments/assets/7eae7d4c-d1b2-4d19-b911-e9751dec8791)


**5. Initialize the Vagrant Environment:**
- Copy the box name **(eurolinux-vagrant/centos-stream-9)**.
  
  ![image](https://github.com/user-attachments/assets/4f5defce-b738-45ab-945d-25cf59cdde97)

- Open your CLI, navigate to the **CentOS** directory, and run the following command to initialize the Vagrant environment: **vagrant init eurolinux-vagrant/centos-stream-9**
- Confirm that the initialization was successful by checking for the creation of the **Vagrantfile** in your directory, using the **ls** command.
  
  ![image](https://github.com/user-attachments/assets/1da9cc6f-f601-4868-a4ff-d24725f6d30a)


**6. Start the Vagrant VM:**
- Use the **vagrant up** command to start the VM
  Vagrant will download the specified box from Vagrant Cloud, store it locally, and create the virtual machine.

  ![image](https://github.com/user-attachments/assets/3f574bc9-7aaf-41ee-b109-1ddf5f3c53c1)


**7. Verify the Box and VM Status:**
- To view the list of available boxes on your local machine, run **vagrant box list**
  
  ![image](https://github.com/user-attachments/assets/077ce969-08c3-4748-8d3b-d41fe998f8f9)

- To check the status of the VM, run **vagrant status**
  
  ![image](https://github.com/user-attachments/assets/901a7650-59df-4b83-83c0-9bf03905ee5b)


**8. Access the VM:**
- Log in to the VM using the **vagrant ssh** command.

   ![image](https://github.com/user-attachments/assets/db2ad2e8-1deb-4e75-8caf-caa50380f003)


