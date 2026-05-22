## AWS S3 CI/CD Workflow

This project uses GitHub Actions to deploy the static e-commerce website to AWS S3.

The workflow first deploys the website files to a staging S3 bucket. After staging is successful, the workflow proceeds to production using GitHub Environments.

Since Amazon S3 does not provide deployment slots like Azure App Service, staging and production were implemented using two separate S3 buckets.

### Staging URL

http://egloy-house-gadgets-staging-2026.s3-website.eu-north-1.amazonaws.com

### Production URL

http://egloy-house-gadgets-site-2026.s3-website.eu-north-1.amazonaws.com
