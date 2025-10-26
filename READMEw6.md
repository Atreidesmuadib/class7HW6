
## Prerequisites
### 1. Ensure  the aws cli ,terraform and .ignorefile are present
### 1.1 Open git bash as an admin (Windows users only)
![Screenshot 2025-10-26 100339](file:///C:/Users/User/Documents/TheoWAF/class7/AWS/Terraform/HW6/hw6pictures/Screenshot%202025-10-26%20100339.png)
### 1.2  run this command 
> curl https://raw.githubusercontent.com/aaron-dm-mcdonald/Class7-notes/refs/heads/main/101825/check.sh | bash>

If you run into this error ![error screen when runnig aaron scripts send to omar](file:///C:/Users/User/Documents/TheoWAF/class7/AWS/Terraform/HW6/hw6pictures/error%20screen%20when%20runnig%20aaron%20scripts%20send%20to%20omar.png)
run this command instead 
> curl --ssl-no-revoke https://raw.githubusercontent.com/aaron-dm-mcdonald/Class7-notes/refs/heads/main/101825/check.sh | bash >

You should see this message ( except the lack of upgrades if terraform is already up to date)
![Screenshot 2025-10-26 105313](file:///C:/Users/User/Documents/TheoWAF/class7/AWS/Terraform/HW6/hw6pictures/Screenshot%202025-10-26%20105313.png)
### 2. In gitbash or your vscode terminal type in the following path 
~/Documents/Theoway/class7/AWS/Terraform

### 3. Verify that you are in the correct folder by looking at the yellow characters 
![Screenshot 2025-10-26 110118](file:///C:/Users/User/Documents/TheoWAF/class7/AWS/Terraform/HW6/hw6pictures/Screenshot%202025-10-26%20110118.png)
### 4. use ls -a command to verify the presence of .gitignore file
![Screenshot 2025-10-26 110407](file:///C:/Users/User/Documents/TheoWAF/class7/AWS/Terraform/HW6/hw6pictures/Screenshot%202025-10-26%20110407.png)
### 5.use mkdir && cd "projectfolder" command to make a sub folder with Terraform & move into it (notice how the path in yellow characters is displaying projectfolder name)
![Screenshot 2025-10-26 110807](file:///C:/Users/User/Documents/TheoWAF/class7/AWS/Terraform/HW6/hw6pictures/Screenshot%202025-10-26%20110807.png)
### 6.type in touch  0-auth.tf &  touch 1-main.tf (creates new files)
![Screenshot 2025-10-26 114009](file:///C:/Users/User/Documents/TheoWAF/class7/AWS/Terraform/HW6/hw6pictures/Screenshot%202025-10-26%20114009.png)
### 7. Type in ls -a +enter to verify 0-auth.tf &  touch 1-main.tf are present ![Screenshot 2025-10-26 11400922](file:///C:/Users/User/Documents/TheoWAF/class7/AWS/Terraform/HW6/hw6pictures/Screenshot%202025-10-26%2011400922.png) 
### 8. type in cd ./.. +enter to return to terraform folder
![Screenshot 2025-10-26 114340](file:///C:/Users/User/Documents/TheoWAF/class7/AWS/Terraform/HW6/hw6pictures/Screenshot%202025-10-26%20114340.png)
### 9 Copy the .gitignore file from terraform to project folder ( cp ./.gitignore "name of project folder") &  cd into project folder
![Screenshot 202502614340](file:///C:/Users/User/Documents/TheoWAF/class7/AWS/Terraform/HW6/hw6pictures/Screenshot%20202502614340.png)






    

