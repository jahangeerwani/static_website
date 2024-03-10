# Static Website Deployment on AWS S3 with CI/CD using AWS CodeBuild and CodePipeline

## Overview

This repository facilitates hosting a static website on AWS S3 with a complete Continuous Integration and Continuous Deployment (CI/CD) pipeline orchestrated manually using AWS CodeBuild and CodePipeline. The manual setup allows for greater customization and control over the deployment process, this can be tried before going with Iac.

## Features

- **Static Website Hosting**: Utilize Amazon S3 to host your static website content.
- **Continuous Integration**: Automatically build and test your website with AWS CodeBuild upon every code commit.
- **Continuous Deployment**: Seamlessly deploy changes to your website with AWS CodePipeline, ensuring rapid and consistent updates.
- **Manual Infrastructure Configuration**: Manually configure AWS resources such as S3 buckets, CodeBuild projects, CodePipeline pipelines, and IAM roles.

## Prerequisites

Before proceeding, ensure you have the following:

- An AWS account with appropriate permissions to create and manage S3 buckets, CodeBuild projects, CodePipeline pipelines, and IAM roles.
- Basic knowledge of AWS services such as S3, CodeBuild, CodePipeline, and IAM.
- Any website template or your website files. (We have used a template here downloaded from https://www.free-css.com/free-css-templates/page288/startup)

## Setup Instructions

Follow these steps to manually set up the CI/CD pipeline for deploying your static website:

1. **Clone the Repository**: Clone this repository to your local machine using Git.
   ```bash
   git clone https://github.com/jahangeerwani/static_website.git
   ```

2. **Configure AWS Credentials**: Ensure you have configured AWS credentials on your local machine with appropriate permissions.

3. **Manual Infrastructure Setup**: Manually create the necessary AWS resources:
   - **S3 Bucket**: Create an S3 bucket to host your static website content.
   - **CodeBuild Project**: Set up a CodeBuild project to build your website.
   - **CodePipeline Pipeline**: Configure a CodePipeline pipeline to orchestrate the deployment process.
   - **IAM Roles**: Create IAM roles with necessary permissions for CodeBuild and CodePipeline.

4. **Configure CodeBuild Buildspec**: Customize the build specifications in the `buildspec.yml` file to define the build steps and artifacts for your website.

5. **Monitor Pipeline**: Monitor the progress of the CodePipeline execution in the AWS Management Console or through the AWS CLI.

6. **Access Website**: Once the pipeline completes successfully, access your static website using the cloudfront URL or custom domain if configured DNS.

## Resources

- [AWS CodeBuild Documentation](https://docs.aws.amazon.com/codebuild)
- [AWS CodePipeline Documentation](https://docs.aws.amazon.com/codepipeline)
- [AWS S3 Documentation](https://docs.aws.amazon.com/s3)
- [AWS IAM Documentation](https://docs.aws.amazon.com/iam)

---
