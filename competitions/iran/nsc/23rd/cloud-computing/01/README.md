# Challenge 01 — Show me you know where things live

This is the first challenge. We are on AWS. I am not asking you to build anything yet.

Before I let you click around in an account, I want to know that the map in your head is right. Region, Availability Zone, who is responsible for what, and who is allowed to touch the account. If those four are fuzzy, the rest of this competition will hurt.

Three questions. Write the answers in Persian, on paper, in your own words. A short answer that is yours beats a long one you copied from a page. If I can see you transcribed a document instead of explaining it, I will treat it as not yours.

At the end of each answer, on the same page, write the references you actually used. A doc title and a link is enough. If you used nothing, write that. Do not leave the bottom of the answer empty.

## How you submit

Write it by hand. Take a photo of each answer. The photo has to be readable: light on the page, the whole page in the frame, your handwriting big enough that I can read the Persian and the references without zooming until it breaks.

Open a pull request with those photos.

In this folder, `competitions/iran/nsc/23rd/cloud-computing/01/`, create a new folder. The folder name is your GitHub username, the same spelling, the same caps. Put the photos in that folder. Name them by question so I do not have to guess:

- `01.jpg` for the first answer
- `02.jpg` for the second
- `03.jpg` for the third

If one answer needs a second page, name it `01-2.jpg`, and so on. The references stay at the end of that answer, not in a separate file.

If your username is `ali-cloud`, I should see something like:

`competitions/iran/nsc/23rd/cloud-computing/01/ali-cloud/01.jpg`

One person, one folder, one pull request. Do not edit this README. Do not put files in someone else's folder. Do not type the answer into GitHub. I want the paper.

## 1. Region and Availability Zone

Tell me what a Region is, and what an Availability Zone is, and how one sits inside the other.

Then answer the part I actually care about. Your users are in one country. The data has to stay in that country. The app still has to stay up if one data center has a bad day. Do you spread it across Regions, or across Availability Zones? Say which one, and why the other one is the wrong tool here.

## 2. What you own, and what AWS owns

AWS runs the building. You run what you put in it. That sentence is too short, so make it real.

Take two cases and tell me, for each one, which side is yours and which side is AWS:

- You launch an EC2 instance and put a web server on it. Who patches the operating system? Who takes care of the physical machine under it?
- You put files in an S3 bucket. Who keeps the disks from dying? Who decides which person in your team can download those files?

I want the split, not the slogan.

## 3. The account is not a shared password

The root user can do everything in the account. You will not use root for this competition, and you will not hand it to a teammate.

In your own words, what is an IAM user, what is an IAM role, and what is an IAM policy? How do the three fit together?

Then a small decision. A teammate needs to read logs for a few days and nothing else. What do you give them, and why is "make another user with full admin and share the password" the wrong answer?
