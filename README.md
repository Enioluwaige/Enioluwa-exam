**AWS EC2 Website Deployment Documentation**

**1. Objective**
To host a personal landing page on an AWS EC2 instance.

**2. Tools and Technologies Used**
Cloud Service: AWS EC2
Operating System: Amazon Linux 2023
Web Server: Apache HTTPD
Files Used: index.html, profile.jpg (from GitHub repository)

3. **Steps Performed**
**Step 1**: Launched an EC2 Instance
Selected the Amazon Linux 2023 AMI.
Configured the security group to allow:
SSH (22): Custom
HTTP (80): Anywhere
HTTPS (443): Anywhere

**Step 2:** Connected to the EC2 Instance
Used SSH to connect:

ssh -i "key.pem" ec2-user@54.75.219.249


**Step 3:** Installed Apache HTTP Server
Updated the system and installed Apache:

yum update -y
yum install -y httpd


Started and enabled Apache:

systemctl start httpd
systemctl enable httpd


**Step 4:** Deployed the Web Content
Downloaded the website files:
wget https://github.com/Enioluwaige/Enioluwa-exam/archive/refs/heads/main.zip
unzip main.zip
mv * /var/www/html/


Verified files in /var/www/html directory.
**Step 5:** Tested the Deployment
Accessed the public IP address in the browser:
arduino
http://54.75.219.249
Confirmed the landing page displayed correctly.

**4. Results**
The website successfully displayed a personal landing page.
Server IP Address: 54.75.219.249

5. Conclusion
The website deployment on AWS EC2 using Amazon Linux and Apache HTTPD was successful. The content from the GitHub repository was hosted and accessible via the public IP.

This was also hosted via netlify 
https://enioluwa-exam.netlify.app/

Kindly see screen shot attached below 

<img width="902" alt="Screenshot 2024-12-18 145111-EXAM - ENIOLUWA" src="https://github.com/user-attachments/assets/e639c839-b12e-4734-a0ad-f1d20843c482" />
<img width="943" alt="Screenshot 2024-12-18 150012-ENIOLUWA GIT HUB" src="https://github.com/user-attachments/assets/54407c21-1817-4695-8d84-95f32837f60a" />
<img width="947" alt="Screenshot 2024-12-18 150135-INSTANCE AWS" src="https://github.com/user-attachments/assets/5ca0cce8-eed4-42f5-92b3-ad64cd9fbb63" />
<img width="950" alt="Screenshot 2024-12-18 150207-AWS-CMDPROMPT" src="https://github.com/user-attachments/assets/ac848b8b-0859-423b-9717-2c850df5b388" />
<img width="960" alt="Screenshot 2024-12-18 150248-INSTALLED-APACHE" src="https://github.com/user-attachments/assets/ec907b93-8449-4883-bad4-158d28940af7" />
<img width="957" alt="Screenshot 2024-12-18 150318-UNZIPPED FILE FOM GIT HUB" src="https://github.com/user-attachments/assets/5913b258-5bea-4136-8ad9-9c669f3f4ce3" />
<img width="959" alt="Screenshot 2024-12-18 150353-SUCCESSFUL LUNCH" src="https://github.com/user-attachments/assets/1e7623be-6483-4361-9d00-4cccc5521398" />




![image](https://github.com/user-attachments/assets/d035f65e-f53d-4e37-8d2f-aa5b6dfa686d)
![image](https://github.com/user-attachments/assets/5d5d4dfd-42f2-4ac4-9abe-2b0c46b65682)
![image](https://github.com/user-attachments/assets/e2640156-3cc1-4465-ac32-32b966d6ffbb)
![image](https://github.com/user-attachments/assets/e19267f1-f778-455b-8d47-5247d1889dfe)
![image](https://github.com/user-attachments/assets/f6fbb279-632b-4a61-a842-7d7a4bba4487)
![image](https://github.com/user-attachments/assets/52aa322f-595e-4b33-9693-121ae8964975)




