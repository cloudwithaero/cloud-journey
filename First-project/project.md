[README(2).md](https://github.com/user-attachments/files/25620702/README.2.md)
<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Host a Website on Amazon S3

**Project Link:** [View Project](http://learn.nextwork.org/projects/aws-host-a-website-on-s3)

**Author:** AERO  
**Email:** cloudwithaero@proton.me

---

![Image](http://learn.nextwork.org/calm_gray_gentle_lynx/uploads/aws-host-a-website-on-s3_5d4474f9)

---

## Introducing Today's Project!

### Project overview

In this project, I will demonstrate using the S3 bucket to hosting static website files  I'm doing this project to learn hosting and using of s3 services from aws 

### Tools and concepts

Services I used were S3 and bucket Key concepts I learnt include 
-how to create an s3 bucket
-what is the ACLs
-how to upload static files
-how to hosting a web files 
-what is the bucket policies 

### Time, challenges, and wins

This project took me approximately 30 mins The most challenging part was to configure the bucket policies and understanding the concepts i've learned today  It was most rewarding to see that webpage is successfully live on the internet 

---

## How I Set Up an S3 Bucket

### What I did in this step

In this step, I will create a general purpose bucket to use  because i'll need it so i can easily upload the website that i want to host easily the static files that i'll upload 

### How long it took to create the bucket

Creating an S3 bucket took me 3 minutes to create the first bucket ever it was so easy with this step guided  

### Region selection

The Region I picked for my S3 bucket was Frankfurt in Germany  because it's the closest one to me so the delay will be less than any other region and time also will be reduced so choose the nearest one to you 


### Understanding bucket name uniqueness

S3 bucket names are globally unique! This means there's no other S3 bucket in the world with the same name i have 

![Image](http://learn.nextwork.org/calm_gray_gentle_lynx/uploads/aws-host-a-website-on-s3_ba6d42ad)

---

## Upload Website Files to S3

### What I did in this step

In this step, I will upload the static file that i'll use in my website because with no files = no website 

### Files I uploaded

I uploaded two files to my S3 bucket - they were index html files that assign the website placeholders and css file and images folder (assets) that will be shown in the website 

### How the files work together

Both files are necessary for this project as html make the base website like text place and images but cant show the image so i need to supply it with the folder that contain the images and assets that will be shown in the website 


![Image](http://learn.nextwork.org/calm_gray_gentle_lynx/uploads/aws-host-a-website-on-s3_a265af88)

---

## Static Website Hosting on S3

### What I did in this step

In this step, I will configure the ACLs to make the website public because if it still private no one will be able to access the website from the internet and then enable the static web hosting because without hosting there's no website 

### Understanding website hosting

Website hosting means storing html and assets files on a powerful computer that make your files visable to the internet (web server )

### How I enabled website hosting

To enable website hosting with my S3 bucket, I go to the proprieties section and scrolled down till i found static web hosting then i enabled it 
 

### Access Control Lists (ACLs)

An ACL is some rules that control who and how anyone that access your bucket and doing any action inside it like upload and delete in breif : set of rules that decides who can get access to a resource.


![Image](http://learn.nextwork.org/calm_gray_gentle_lynx/uploads/aws-host-a-website-on-s3_c22c54c0)

---

## Bucket Endpoints

### Understanding bucket endpoint URLs

Once static website is enabled, S3 produces a bucket endpoint URL, which is URL. It lets people visit your S3 bucket's files as a website.

### What I saw when I tested the endpoint

When I first visited the bucket endpoint URL, I saw error 403 forbidden and access is denied  . The reason for this error was that even if i have enable "Block all public access " i have to make the objects public too it's still private 

![Image](http://learn.nextwork.org/calm_gray_gentle_lynx/uploads/aws-host-a-website-on-s3_22ce4daf)

---

## Success!

### What I did in this step

In this step, I will make the objects i've uploaded to be public so it cane be accessed by anyone on the internet  because if it still private this means no one can access the web i just hosted on the web server 

### How I resolved the 403 error

To resolve this 403 Forbidden error, I first selected all the objects that i want to make public and then clicked on the actions button and choose the "making them public using ACLs " that's it all

![Image](http://learn.nextwork.org/calm_gray_gentle_lynx/uploads/aws-host-a-website-on-s3_5d4474f9)

---

## Bucket Policies

### What I did in this extension

In this project extension I'm about to using the ACLs code to edit who can access the files and edit on them like delete it I'm doing this so that no one can delete my projects i've made 

### Understanding bucket policies

An alternative to ACLs are bucket policies, which are. effective some codes that define who and what they can do on my bucket The benefit of using bucket policies is while ACLs are useful for general purpose  

![Image](http://learn.nextwork.org/calm_gray_gentle_lynx/uploads/aws-host-a-website-on-s3_sm2sm2sm)

### What my bucket policy does

My bucket policy was to block any one from deleting the (index.hmtl) file I tested this by trying to delete the file i want to protect  and saw the error message that tell me that access is denied and failed to delete this file 

---

---
