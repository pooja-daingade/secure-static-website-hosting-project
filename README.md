# Secure Static Website Hosting Project

## Project Overview

This project demonstrates the deployment of a static website on AWS with secure HTTPS access using Amazon S3, Amazon CloudFront, AWS Certificate Manager (ACM), and Amazon Route 53.

The website files are stored in an Amazon S3 bucket, CloudFront is configured for content delivery, ACM provides the SSL/TLS certificate, and Route 53 manages the custom domain routing.

## AWS Services Used

- Amazon S3 – Stores the static website files
- Amazon CloudFront – Delivers website content and enables HTTPS
- AWS Certificate Manager (ACM) – Provides the SSL/TLS certificate
- Amazon Route 53 – Manages DNS and custom domain routing

## Architecture

<img width="1536" height="1024" alt="architecture-diagram png" src="https://github.com/user-attachments/assets/b1088906-40c8-4e1a-b73f-28dbdf6f2da6" />


## Domain

`https://dev.poojadaingade.shop`

## Key Configuration

- S3 bucket: `pooja-static-web-bucket`
- AWS Region: `ap-south-1` (Mumbai)
- S3 Versioning: Enabled
- Block All Public Access: Enabled
- CloudFront distribution: `static-web-hosting`
- Default Root Object: `index.html`
- SSL/TLS Certificate: AWS Certificate Manager
- DNS: Amazon Route 53
- HTTPS: Enabled

## Project Workflow

1. Created an S3 bucket and uploaded the static website files.
2. Enabled S3 Versioning and Block All Public Access.
3. Requested and validated an SSL/TLS certificate using ACM.
4. Created a CloudFront distribution with the S3 bucket as the origin.
5. Configured `index.html` as the default root object.
6. Added the custom domain to CloudFront and attached the ACM certificate.
7. Configured Route 53 to route the custom domain to CloudFront.
8. Verified the website using HTTPS.

## Website Files

The `website` directory contains the static website files:

- `index.html`
- `style.css`

## Documentation

Detailed step-by-step implementation with screenshots is available in:

**Secure_Static_Website_Hosting_with_HTTPS_on_AWS.pdf**

## Final Result

The static website is successfully deployed and accessible through the custom domain using HTTPS:

`https://dev.poojadaingade.shop`

## Author

**Pooja Daingade**
