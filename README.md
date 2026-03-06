# AWS Static Website Hosting Project

## Author

Aly Kane  
Cybersecurity Student

## Overview
## Overview

This project demonstrates how to deploy and deliver a static website using Amazon Web Services (AWS). The website was first hosted using Amazon S3 static website hosting and then placed behind AWS CloudFront to enable HTTPS encryption and improve website delivery through a global content delivery network (CDN).

The purpose of this project was to gain hands-on experience with cloud storage, access control, static website hosting, and CDN-based content delivery using AWS services.

## Technologies Used
- Amazon S3
- AWS Management Console
- HTML
- Content Delivery Network (CDN)
- HTTPS

## Project Steps

###  Created a static webpage
I created a simple HTML webpage called `index.html` using VS Code.

###  Created an S3 bucket
A new S3 bucket was created in AWS to store the website files.


### Uploaded website files
The index.html file was uploaded to the bucket.

###  Enabled Static Website Hosting
Static website hosting was enabled in the bucket properties.



###  Configured public access
Public access settings were modified to allow users to access the website.

###  Added bucket policy
A bucket policy was created to allow public read access to objects in the bucket.

## CloudFront CDN and HTTPS

To improve performance and security, the static website was placed behind an AWS CloudFront distribution.

CloudFront acts as a Content Delivery Network (CDN) that delivers website content through global edge locations and enables HTTPS encryption.

### Configuration Steps

- Created a CloudFront distribution
- Selected the S3 bucket as the origin
- Allowed CloudFront private access to the S3 bucket
- Used recommended cache settings for S3 content
- Configured the default root object to load the homepage
- Deployed the distribution so the website can be delivered through CloudFront

### Result

The website is now served through CloudFront over HTTPS.

User → CloudFront CDN → S3 Bucket




## What I Learned
- How Amazon S3 stores objects
- How static website hosting works in AWS
- How bucket policies control access
- Basic cloud deployment workflow# was-static-website-project
Hosting a static website using AWS S3 with public access policies.

## Project Architecture

The website is deployed using Amazon S3 for storage and AWS CloudFront for secure content delivery.

Traffic flow:

User → CloudFront CDN → Amazon S3

CloudFront retrieves the website files from the S3 bucket and delivers them securely to users over HTTPS.

## Architecture Diagram
                +--------------------+
                |       Users        |
                |  Web Browser /     |
                |  Internet Traffic  |
                +---------+----------+
                          |
                          | HTTPS
                          v
                +--------------------+
                |    AWS CloudFront  |
                |  Content Delivery  |
                |       Network      |
                +---------+----------+
                          |
                          | Secure origin request
                          v
                +--------------------+
                |     Amazon S3      |
                |  Static Website    |
                |   File Storage     |
                +--------------------+
## Live Endpoints

### CloudFront Endpoint (Secure Production Delivery)

This is the primary endpoint used to access the website through CloudFront with HTTPS enabled.

https://d1bk4o3fq471xc.cloudfront.net

### S3 Static Website Endpoint

This endpoint was used during the initial deployment when the website was hosted directly through Amazon S3 static website hosting.

http://alykane-aws-project1.s3-website.us-east-2.amazonaws.com
