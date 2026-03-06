# AWS Static Website Hosting Project

## Overview
This project demonstrates how to deploy a static website using Amazon S3.

The goal was to understand how cloud storage, access policies, and static website hosting work in AWS.

## Technologies Used
- Amazon S3
- AWS Management Console
- HTML

## Project Steps

### 1. Created a static webpage
I created a simple HTML webpage called `index.html` using VS Code.

### 2. Created an S3 bucket
A new S3 bucket was created in AWS to store the website files.

Bucket name example:
alykane-aws-project1

### 3. Uploaded website files
The index.html file was uploaded to the bucket.

### 4. Enabled Static Website Hosting
Static website hosting was enabled in the bucket properties.

Index document:
index.html

### 5. Configured public access
Public access settings were modified to allow users to access the website.

### 6. Added bucket policy
A bucket policy was created to allow public read access to objects in the bucket.

## Result
The website was successfully deployed and accessible through the AWS static website endpoint.

## Example Endpoint
http://your-bucket-name.s3-website-region.amazonaws.com

## What I Learned
- How Amazon S3 stores objects
- How static website hosting works in AWS
- How bucket policies control access
- Basic cloud deployment workflow# was-static-website-project
Hosting a static website using AWS S3 with public access policies.
