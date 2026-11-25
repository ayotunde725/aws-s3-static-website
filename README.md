
# AWS S3 Static Website

A personal cloud portfolio website by Yusuf Ayodeji, hosted on Amazon S3 and delivered through Amazon CloudFront.

## Live demo
- GitHub Pages: https://https://github.com/ayotunde725.github.io/aws-s3-static-website/
- AWS (S3 + CloudFront): coming soon

## What this project shows
How to host a static website on AWS and serve it fast and securely over HTTPS, using the same building blocks real companies use for their websites.

## Architecture
Visitor -> CloudFront -> S3 bucket (index.html, error.html)

Architecture diagram: coming soon

## AWS services used
- Amazon S3: stores the website files
- Amazon CloudFront: keeps fast copies close to visitors and adds HTTPS
- IAM: a helper user with limited permissions instead of the root login
- AWS Budgets: an alert so I never get a surprise bill

## Progress
- [x] Built the website (index.html and error.html) and pushed it to GitHub
- [ ] Created the S3 bucket
- [ ] Uploaded the files and turned on static website hosting
- [ ] Put CloudFront in front of the bucket with HTTPS
- [ ] Added screenshots
- [ ] Deleted the resources to avoid charges

## Cost
To be updated when the project is finished.

## What I learned
To be updated when the project is finished.

## Author
Yusuf Ayodeji
