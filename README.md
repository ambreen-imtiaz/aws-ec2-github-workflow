# AWS EC2 GitHub Workflow Using Windows Command Prompt

## Project Overview

This project demonstrates a complete Git and GitHub workflow using an AWS EC2 Ubuntu instance. The project includes launching an AWS EC2 instance, connecting securely through SSH from Windows Command Prompt, configuring Git, managing a repository, creating branches, committing changes, merging updates, and pushing changes to GitHub.

## Technologies Used

* AWS EC2
* Ubuntu Linux
* Windows Command Prompt
* Git
* GitHub
* SSH

## Project Objectives

* Launch and configure an Ubuntu EC2 instance on AWS.
* Connect securely to the EC2 instance using SSH from Windows Command Prompt.
* Install and configure Git on Ubuntu.
* Connect a local Git repository with GitHub.
* Practice Git version control workflow including commits, branches, merging, and pushing changes.

## Project Implementation

### 1. AWS EC2 Setup

* Created an Ubuntu EC2 instance on AWS.
* Configured SSH access using a private key (.pem file).
* Connected to the EC2 instance using Windows Command Prompt.

### 2. Linux Environment Verification

The following commands were used to verify the EC2 environment:
bash
whoami
hostname
pwd
ls -a

### 3. Git Installation and Configuration

Installed Git on the Ubuntu EC2 instance:

bash
sudo apt update
sudo apt install git -y

Verified Git installation:

bash
git --version

Configured Git user details:

bash
git config --global user.name "Ambreen-Imtiaz"
git config --global user.email "ambreenimtiaz4321@gmail.com"

Checked Git configuration:

bash
git config --list

### 4. Repository Management

Managed the Git repository and connected it with GitHub:

bash
git clone <repository-url>
git status
git add .
git commit -m "Add initial project document"
git push -u origin main

These commands were used to track changes, create commits, and upload project updates to GitHub.

### 5. Branch Workflow

Created and managed a feature branch to practice collaborative development:

bash
git branch feature-update
git checkout feature-update
git add.
git commit -m "Add feature update file"
git push -u origin feature-update

Merged feature changes into the main branch:

bash
git checkout main
git merge feature-update
git push

### 6. Git Remote and History Verification

Verified the connection between the local repository and GitHub:

bash
git remote -v

Reviewed commit history:

bash
git log --oneline --decorate --graph --all

Checked final repository status:

bash
git status

## Project Screenshots

### EC2 Connection and Linux Environment

![EC2 Connection](01_EC2_Connection_and_Linux_Environment.png)

### Git Installation and Configuration

![Git Configuration](02_Git_Installation_and_Configuration.png)

### Git Status and Branch Workflow

![Git Branch Workflow](03_Git_Status_and_Branch_Workflow.png)

### Git History, Remote Repository, and Final Status

![Git History](04_Git_History_Remote_and_Final_Status.png)

## Skills Demonstrated

* AWS EC2 deployment and configuration
* Linux command-line operations
* SSH remote connection
* Git version control
* GitHub repository management
* Branching and merging workflow
* Command-line troubleshooting

## Learning Outcome

Through this project, I gained practical experience with cloud-based development environments, Linux administration, Git version control, and GitHub collaboration workflows. This project improved my understanding of how developers manage code changes, maintain repositories, and use version control systems in real-world DevOps environments.


