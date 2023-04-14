# Amazon machine image

- a way of storing previous instances created on AWS, allows you to 
make iterations in development of instances, but these AMIs are immutable.

![](architecture_ami_instance.png)

### How to create an AMI

Navigate to your instance and select it, click actions, 
image and templates, create image. 

![](image1.png)

Add image name and desc, it is good practice to use a good naming convention
for this and to add a description of the image so if someone new
were to use it they do details about it.

![](image2.png)

You will be presented with alot of the options you were given when you first created the 
instance, the OS image will be selected for you.

![](image8.png)

You will need to add the key pair to allow you to access the instance.

![](image9.png)

Within network settings, you can either select security group you have previously made
or decide to create a new one, in this case we chose a existing one.

![](image10.png)

Optional to change size, add volumes and add tags, click "create image".

### How to access and Launch AMI

navigate to images section and select ami's. 

![](image3.png)

Once you have located your AMI, you can add a name/tag by hovering over
name and select to edit 

![](image4.png)

Before we can launch our AMI, we need to make sure the status is "Available".

![](image5.png)

Now, all that's left to do is Launch the instance from our AMI.

![](image6.png)

### How to access and share AMI 

Connect to instance and follow aws prompts and see previous readme for more documentation

![](image11.png)

Moving to our Git Bash window, if we enter this command, we will be asked 
to log in using ubuntu and not root, meaning we need to run the 
same command replacing "root" with ubuntu.

![](image12.png)

A welcome message will show you have accessed this image.
It's important to note that you can also make AMI's to sell or use ones being sold
on the AMI catalog.




### IAM identity access management - LPA least privileged access (Need to now Basis)

Create accounts for others, grant and deny permissions depending on personal,
account management.

- navigate to IAM dashboard
- search for the user you want to check their permissions

#### to add new policy 

- search for the policy and request for the permission





