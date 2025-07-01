This project contains a simple React application that is automatically built and deployed to an AWS S3 bucket using GitHub Actions.

 Tech Stack
React – Frontend Framework

GitHub Actions – CI/CD Automation

AWS S3 – Static Website Hosting

GitHub Actions Workflow
The pipeline performs the following steps:

Trigger: Runs on push to master branch.

Checkout: Clones the repository code.

Setup Node.js: Uses Node version 17.9.1.

Install Dependencies: Runs npm install inside the client/ directory.

Build React App: Builds the app using CI=false npm run build to avoid ESLint warning errors.

Deploy to AWS S3: Uses jakejarvis/s3-sync-action to sync the build folder to your configured S3 bucket.

code i used open sopurce from github this is just demo project for my work
