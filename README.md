# GitHub Actions - EC2 Apache Deployment

## Project Overview

This is a simple CI/CD demo project where an HTML webpage is
deployed to an Amazon EC2 instance using GitHub Actions.

Whenever changes are pushed to the GitHub repository, GitHub Actions connects
to the EC2 instance and deploys the updated HTML file to the Apache web server.

## Architecture

Developer
↓
GitHub Repository
↓
GitHub Actions
↓
EC2 Instance
↓
Apache Web Server
↓
Web Page


## Tools Used

* Git
* GitHub
* GitHub Actions
* Apache
* Linux
* AWS EC2


## GitHub Secrets

The following sensitive values are stored in GitHub Actions Secrets:

* `EC2_HOST` – EC2 public IP address
* `EC2_USER` – EC2 SSH username
* `EC2_PRIVATE_KEY` – EC2 private SSH key

Private keys and credentials are not stored directly in the source code.

## Apache Verification

After successful deployment, open:

```text
http://<EC2-PUBLIC-IP>
```

The updated HTML page should be displayed.

## Result

The project demonstrates a basic CI/CD workflow where:

**GitHub Push → GitHub Actions → EC2 → Apache → Updated Web Page**

## Key Learnings

* Created an EC2 instance.
* Installed and configured Apache.
* Used Git and GitHub.
* Created a GitHub Actions workflow.
* Used GitHub Secrets for sensitive information.
* Automated deployment to EC2.
* Verified the application through the EC2 public IP.


## created by 
jaweriya mmahin



