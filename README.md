DEVOPS
ASSIGNMENT 1
Installation of Oracle VirtualBox:
1.	Download VirtualBox: 
 Go to virtualbox.org, download it for your OS.
2.	Install VirtualBox: 
 Run the installer and follow the steps (Windows/macOS/Linux).
3.	Create a Virtual Machine:
o	Open VirtualBox, click New.
o	Name it, select OS type, allocate RAM.
o	Create a virtual hard disk.
4.	Install the OS:
o	Start the VM, select your OS installation ISO, and complete the setup.
OUTPUT:
 


 












ASSIGNMENT 2

Installation of Nginx.
Task Description:
This task involves creating a Jenkins Freestyle job that automates the installation of Nginx on an Ubuntu server using the command sudo apt-get install -y nginx. This automation ensures consistent server setup and can be easily repeated, making it ideal for automated environments.
________________________________________
Steps:
1.	Update Package List:
o	Run the following command to update the package list: 
o	sudo apt update
2.	Install Nginx:
o	Install Nginx using the following command: 
o	sudo apt-get install -y nginx
3.	Verify Installation:
o	Check if Nginx is running with the command: 
o	systemctl status nginx
4.	Create Jenkins Freestyle Job:
o	In Jenkins, click New Item and create a Freestyle project (e.g., Install_Nginx).
5.	Configure Job:
o	Add a build step of type Execute shell.
o	In the shell command box, enter: 
o	sudo apt update
o	sudo apt-get install -y nginx
6.	Save and Run Job:
o	Save the job and click Build Now to run it.

7.	Check Console Output:
o	After the job completes, view the Console Output to confirm the successful installation of Nginx.

      OUTPUT:

        










ASSIGNMENT  3
CI/CD Pipeline Setup Using Jenkins
Task Description:
This task involves setting up a Continuous Integration and Continuous Deployment (CI/CD) pipeline using Jenkins to automate the build, test, and push process of a containerized web application. The pipeline integrates GitHub for source code management, Docker for containerization, and a container registry (such as Docker Hub) for storing the container image.
________________________________________
Steps to Set Up the CI/CD Pipeline:
1.	Install Jenkins:
o	Ensure Jenkins is running and install necessary plugins (Git, Docker).
2.	Create a New Pipeline Job:
o	Create a new Pipeline job in Jenkins to automate the build, test, and deployment process.
3.	Configure the GitHub Repository:
o	Link your GitHub repository to Jenkins to automatically pull the latest code.
4.	Write the Pipeline Script (Jenkinsfile):
o	Define stages in the Jenkinsfile: 
	Clone Repository: Pull the latest code from GitHub.
	Build Docker Image: Build the image using Docker.
	Push Docker Image: Push the image to a container registry (e.g., Docker Hub).
5.	Add Docker Credentials (if needed):
o	Add Docker credentials to Jenkins if using a private registry for authentication.
6.	Trigger the Pipeline:
o	Trigger the pipeline manually or set up GitHub webhooks for automatic triggers on code changes.

 OUTPUT:
        



