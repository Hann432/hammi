





.




##PROJECT 4: BACKUP AND RESTORE - OF EC2 INSTANCES 🤓


.

.
![alt text](https://sageaccountssolutions.co.uk/wp-content/uploads/2018/09/backup_animation.gif)



.



..

##INTRODUCTION: 

######This team project exemplifies our collaborative effort in fortifying our disaster recovery capabilities by implementing an effective EC2 backup and restore process in AWS. By emphasizing teamwork, best practices, and shared decision-making, we've strengthened our skills in maintaining system reliability and optimizing resource utilization.

######Our team collaborated to enhance disaster recovery capabilities by establishing a robust EC2 backup and restore system in AWS.


.

##1.  How To Create A Windows Server EC2 instance
.
.

  
![alt text](https://miro.medium.com/v2/resize:fit:828/format:webp/1*YovzCTXsgM3uKnqCzV9Cew.gif)


Creating a Windows Server EC2 (Elastic Compute Cloud) instance on AWS (Amazon Web Services) involves several steps. Here's a general guide to help you set up a Windows Server EC2 instance:
.
.
.
####1. Sign in to the AWS Management Console:
- Go to the AWS Management Console.
- Sign in to your AWS account.
.
####2. Navigate to EC2:
- In the AWS Management Console, go to the "Services" dropdown, and select "EC2" under the "Compute" section.
.
####3. Launch an Instance:
- Click on the "Instances" link in the left navigation pane.
- Click the "Launch Instance" button.
.
####4. Choose Windows Server Machine Image:
- Select the desired Windows Server AMI. These are pre-configured images with Windows Server.
- You can choose the appropriate version and edition of Windows Server based on your requirements.
.
####5. Choose an Instance Type:
- Select the instance type based on your performance needs. The available options vary in terms of CPU, memory, and networking capacity.
.
####6. Configure Instance:
- Set the number of instances you want to launch.
- Configure other details like network settings, subnet, auto-assign public IP, and more.
.
####7. Add Storage:
Specify the size of the root volume (C: drive) for your Windows instance.
You can also add additional volumes if needed.
.
####8. Add Tags (Optional):
- Add any tags to your instance for better organization and management.
.
####9. Configure Security Group:
- Create or select a security group. This is a virtual firewall that controls inbound and outbound traffic to your instance.
- Ensure that RDP (Remote Desktop Protocol) is allowed so you can connect to the Windows instance.
.
####10. Review and Launch:
- Review your configuration to ensure everything is set up correctly.
- Click "Launch" to start the instance creation process.
.
####11. Create a Key Pair (if not using existing):
- If you don't have an existing key pair, you'll need to create one. 
- This is used for secure access to your instance.
Save the key pair (.pem file) securely.
.
####12. Launch Instance:
- Click "Launch Instances" to create your Windows Server EC2 instance.
.
####13. View Instances:
- Once the instance is launched, go back to the EC2 dashboard and navigate to "Instances" to view your newly created instance.
.
####14. Connect to the Instance:
- Use a Remote Desktop Client to connect to the Windows Server instance using the public IP address and the key pair (.pem file) you created.
.
####15. Configure Windows Server:
- Complete the Windows setup process by providing necessary information, setting passwords, etc.





.
.
.

##Using AMI To Backup an EC2 Instance
.

.
###2. Create a Windows Server 2022 Machine Image:
.

![alt text](https://miro.medium.com/v2/resize:fit:828/format:webp/1*3ikIiLV0VljykbThPdPehA.png)



####Step 1: Navigate to the EC2 Dashboard
- In the AWS Management Console, go to the EC2 Dashboard.
.
####Step 2: Select your Instance

- In the Instances view, select the EC2 instance you want to back up.
.
####Step 3: Create an AMI

- With your instance selected, click on the "Actions" button, then navigate to "Image and templates" and choose "Create Image."
- Provide a unique name and description for the image.
- Click "Create Image."
.
####Step 4: Monitor the AMI Creation

- The AMI creation process may take some time. You can monitor the progress in the "AMIs" section of the EC2 Dashboard.
.
####Step 5: Launch from AMI (Optional)

- Once the AMI is created, you can launch a new instance from it at any time.
.


###2. Create an Amazon EBS Snapshot:

.


####Step 1: Navigate to the EC2Dashboard
.
- In the AWS Management Console, go to the EC2 Dashboard.
.
####Step 2: Select Volumes
.
- In the left navigation pane, click on "Volumes" under "Elastic Block Store."
.
####Step 3: Select the Volume
- Find the volume attached to your. EC2 instance and select it.
.
####Step 4: Create Snapshot

- With the volume selected, click on the "Actions" button, then choose "Create Snapshot."

- Provide a meaningful name and description for the snapshot.

- Click "Create Snapshot."
.
####Step 5: Monitor Snapshot Creation
 .
- You can monitor the progress in the "Snapshots" section of the EC2 Dashboard.
.
####Step 6: Restore from Snapshot (Optional)

- If needed, you can create a new EBS volume from the snapshot and attach it to a new EC2 instance.
- Tips and Best Practices:


- Ensure your applications are in a consistent state before taking a snapshot to avoid data corruption.

.
.
##3. How To Restore Windows EC2 Instance
.

![alt text](https://cdn.dribbble.com/users/665790/screenshots/16941214/media/4fd157144032c137fb3bf4e18c3d5fd7.gif)



- AMI Selection: Collectively chose the appropriate AMIs for restoration purposes within the EC2 Dashboard.

- New Instance Launch: Collaborated on launching new instances from selected AMIs, considering various instance details and network settings.
Instance Settings 

- Configuration: Shared responsibility in configuring settings, including storage options and tagging conventions.

- Instance Launch: Collaboratively launched instances and established necessary access protocols (SSH/RDP). Find the AMI you want to use for restoration.


.

####1. AWS Documentation:
.
- Amazon EC2 Documentation: The official documentation is a comprehensive resource for understanding EC2, including backup and restore concepts.
.
####2. AWS Well-Architected Framework:

- Well-Architected Framework - Security Pillar: This provides best practices for securing your applications, including data backup and recovery.
.
####3. AWS Free Tier:
- AWS Free Tier: If you're new to AWS, take advantage of the free tier to practice creating instances, taking snapshots, and understanding the costs associated.
.
####4. AWS Training and Certification:

- AWS Training: AWS offers various training courses. Look for courses related to EC2, data management, and security.
.
####5. YouTube Tutorials:

- Search for tutorials on YouTube from reputable AWS trainers and channels. Many instructors provide step-by-step guides for EC2 instance backup and restore.
.
####6. Online Courses:
- Platforms like Coursera, Udacity, and A Cloud Guru offer courses on AWS. Look for courses specifically covering EC2 backup and recovery.
.
####7. Blogs and Articles:

- Read blogs and articles on the AWS Blog and other reputable tech blogs for in-depth discussions on EC2 backup strategies.
.
####8. Forums and Communities:

- Participate in AWS forums, such as the AWS Developer Forums or Stack Overflow, to learn from the experiences of other AWS users.
.
####9. Hands-On Practice:
- The best way to learn is by doing. Practice creating EC2 instances, taking snapshots, and restoring instances in a sandbox or development environment.







.

.













Presentation Produced By;


,
#####Jamilla, Hani, Betrand, and Khalid 

.

.
#


