# AWS S3 Static Website

A personal cloud portfolio website by Yusuf Ayodeji, hosted on Amazon S3 and delivered through Amazon CloudFront.

## Current status
**In progress: waiting for AWS CloudFront account verification.**

The website files are uploaded to Amazon S3. When I tried to create the CloudFront distribution, AWS asked me to verify my new account before allowing CloudFront resources, which is a standard step for new accounts. I have opened a support case with AWS and will finish the CloudFront setup as soon as it is approved.

## Live demo
- GitHub Pages: https://ayotunde725.github.io/aws-s3-static-website/
- AWS (S3 + CloudFront): coming soon, pending verification

## What this project shows
How to host a static website on AWS and serve it quickly and securely over HTTPS, using the same building blocks real companies use.

## Architecture
Visitor -> CloudFront (HTTPS) -> private S3 bucket (index.html, error.html)

The bucket stays private. Only CloudFront can read from it, using Origin Access Control (OAC), so nobody can bypass CloudFront and read the bucket directly.

## AWS services used
- Amazon S3: stores the website files
- Amazon CloudFront: delivers the site fast over HTTPS
- Origin Access Control: keeps the bucket private
- IAM and MFA: protects the account
- AWS Budgets: alerts me before costs grow

## Progress
- [x] Built the website (index.html and error.html) and pushed it to GitHub
- [x] Published a live copy with GitHub Pages
- [x] Secured the AWS account with MFA and a budget alert
- [x] Created the S3 bucket and uploaded the files
- [ ] Create the CloudFront distribution (waiting for AWS account verification)
- [ ] Lock the bucket with Origin Access Control
- [ ] Add screenshots of the finished setup
- [ ] Delete the resources to avoid charges

## What I learned so far
- A new AWS account may need extra verification before CloudFront can be used, and AWS Support is the route to resolve it.
- S3 has two endpoints: the bucket endpoint, which works with a private bucket and OAC, and the website endpoint, which needs a public bucket. I chose the bucket endpoint for better security.

## Author
Yusuf Ayodeji
