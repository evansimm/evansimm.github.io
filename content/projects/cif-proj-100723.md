---
title: Cloud is free
dateMonthYear: October 7, 2023
description: Cloud is free is a platform dedicated to assisting individuals in setting up practical projects with interactive, detailed documentation while making the most of the Free Tier offerings from various Cloud platforms.
type: page
topic: project
author: Evan
#link: "https://www.mathbraintrainer.com"
#image: "/images/braintrainer.png"
---

## Introduction
What is **Cloud is free**? Cloud is free is a platform dedicated to assisting individuals in setting up practical AWS projects with interactive, detailed documentation while making the most of the Free Tier offerings from various Cloud platforms.

At the time of this post, Cloud is free offers 3 projects of varying complexity, with more projects in the pipeline. The projects are: Hosting a Static Website in, creating a Severless Sending Application, and managing and visualizing an RDS database using ECS containers.

## Project 1: Static Website Hosting
*Task: Create a static website using S3, CloudFront, Route 53, and ACM.*
![Project 1 Diagram](static/images/cif-proj1-md.png)
Since I've previously built a static website in AWS for the **Cloud Resume Challenge** I avoided following the instructions step by step and tried to use alternative steps to complete the project where possible. I used CloudShell to set up the S3 buckets (for static hosting and redirection). I used CloudShell again to create a hosted zone in Route 53, gaining extra experience with CLI commands in AWS. To secure my domain, I purchased an affordable one from porkbun.com and configured it in both Porkbun's dashboard and Route 53. I also opted to create and use a single CloudFront distribution rather than two separate ones, as in my research I determined there was very little benefit to having separate distributions.

Overall, Project 1 was a valuable refresher on static website creation, allowing me to use skills I acquired during the Cloud Resume Challenge.

## Project 2: Serverless Sending Application
*Task: Create a serverless application that sends SMS and email notifications using S3, API Gateway, Lambda, Step Functions, SNS, and SES.*
![Project 2 Diagram](static/images/cif-proj2-md.png)
This project combines S3, API Gateway, Lambda, Step Functions, SNS, and SES. I encountered a minor setback as I didn't have a registered toll-free number to use for sending SMS messages, but the email functionality worked flawlessly in my tests. 

This project gave me great exposure to some of the serverless services AWS offers, and I look forward to exploring them further in future projects.

## Project 3: Database and Containers
*Task: Create an RDS database and manage it using ECS containers.*
![Project 3 Diagram](static/images/cif-proj3-md.png)
Project 3 explores VPCs, subnets, RDS databases, EC2 instances, EBS volumes, ECS containers, and EFS. One challenge I faced was following the project's instructions to the letter resulting in the Metabase container being unable to be implemented. It appears that the Metabase container image now demands slightly more resources than when Cloud is free was initially created. Allocating about 20 MB of additional RAM to Metabase seemed to resolve the problem, allowing me to complete the project successfully.

Project 3 pushed my boundaries a bit, offering an intriguing and realistic architecture to practice with. It is the most challenging project of the three, but it is also the most rewarding.

## Conclusion
Cloud is free is your go-to resource for hands-on cloud project guidance. Each project provides invaluable learning experiences, and I can't wait to explore and build more projects that they create.