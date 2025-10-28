


## Prerequisites
### 1. Ensure  the aws cli ,terraform and .ignorefile are present
### 1.1 Open git bash as an admin (Windows users only)
![screenshot (9)](./hw6pictures/screenshot%20(9).png)
### 1.2  run this command 
> curl https://raw.githubusercontent.com/aaron-dm-mcdonald/Class7-notes/refs/heads/main/101825/check.sh | bash>

If you run into this error ![error screen when runnig aaron scripts send to omar](file:///C:/Users/User/Documents/TheoWAF/class7/AWS/Terraform/HW6/hw6pictures/error%20screen%20when%20runnig%20aaron%20scripts%20send%20to%20omar.png)
run this command instead 
> curl --ssl-no-revoke https://raw.githubusercontent.com/aaron-dm-mcdonald/Class7-notes/refs/heads/main/101825/check.sh | bash >

You should see this message ( except the lack of upgrades if terraform is already up to date)
![screenshot (2)](./hw6pictures/screenshot%20(2).png)
### 2. In gitbash or your vscode terminal type in the following path 
![screenshot (3)](./hw6pictures/screenshot%20(3).png)

### 3. Verify that you are in the correct folder by looking at the yellow characters 
![screenshot (4)](./hw6pictures/screenshot%20(4).png)
### 4. use ls -a command to verify the presence of .gitignore file
![screenshot (41)](./hw6pictures/screenshot%20(41).png)
### 5.use mkdir && cd "projectfolder" command to make a sub folder with Terraform & move into it (notice how the path in yellow characters is displaying projectfolder name)
![screenshot (5)](./hw6pictures/screenshot%20(5).png)
### 6.type in touch  0-auth.tf &  touch 1-main.tf (creates new files)
![screenshot (6)](./hw6pictures/screenshot%20(6).png)
### 7. Type in ls -a +enter to verify 0-auth.tf &  touch 1-main.tf are present 
![screenshot 61](./hw6pictures/screenshot61.png)

### 8. go to https://registry.terraform.io/ & click browse providers
![Screenshot62](./hw6pictures/Screenshot62.png)

### 9. Click on the AWS logo
![aws registry](./hw6pictures/awsproviderstf.png)

### 10. Click on the purple documentation button on the right hand side
![tf aws documentation](./hw6pictures/tfregistrydoc.png)

### 11. Scroll down to example usage & copy the following code block
![authfilecode](./hw6pictures/authfilecode.png)

### 12. If you haven't opened vs yet return to git bash 
![gitbash](./hw6pictures/gitbash.png)
### 13 Type in  cd ./oct26 (or your project name after the slash)
![gitbash 2](./hw6pictures/gitbash2.png)

### 14. To open vscode type in code .+enter
![gitvs](./hw6pictures/gitvs.png)

### 15. Click on left side on 0.auth.tf
![vscodeedit](./hw6pictures/vscodeedit.png)
### 16. Paste the code we copied in Step 11  (make sure to edit your default region unless it's us-east-1)
![pastingcode](./hw6pictures/pastingcode.png)

### 17. Return to the terraform registry web page & type aws vpc in the left side menu
![getmaincode](./hw6pictures/getmaincode.png)
### 18 Under the resources dropdown left click on aws_vpc
![tfreg](./hw6pictures/tfreg.png)

### 19.0 Click copy  on the code block right under Example Usage
![maincode](./hw6pictures/maincode.png)

### 20.00 Return to vs code & left click on 1-main.tf
![mainvs](./hw6pictures/mainvs.png)

### 21.00 Paste  the code you copied in  step 19 in the text field show in image below
!![codevv](./hw6pictures/codevv.png)

### 22. type in cd ./.. +enter to return to terraform folder
![screenshot (7)](./hw6pictures/screenshot%20(7).png)
### 23. Copy the .gitignore file from terraform to project folder ( cp ./.gitignore "name of project folder") 
![screenshot(11)](./hw6pictures/screenshot(11).png)
### 24. type in cd ./oct26 or (replace oct26 by project folder name)
![screenshot 12](./hw6pictures/screenshot12.png)
### 25. Type in terraform init +enter
![screenshot 13](./hw6pictures/screenshot13.png)
### 26.Type in terraform validate + enter (results should look like image below)
![screenshot 14](./hw6pictures/screenshot14.png)
### 27.Type in terraform plan+enter
![screemshot 15](./hw6pictures/screemshot15.png)

## successful terraform apply
![terraformapply](./hw6pictures/terraformapply.png)





**extra comment do not modify tfstate, .terraform.lock.hcl & .terraform folder. Messing them up with can break your infrastructure & will get you fired.** 
=======











  
