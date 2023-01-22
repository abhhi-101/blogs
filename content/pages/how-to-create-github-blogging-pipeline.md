Title: How to create your own GitHub powered blogging website for free
Date: 2023-01-21 10:20
Tags: host on github, free blogging website
Category: stories
Slug: how-to-create-github-blogging-pipeline
Authors: Abhishek Birdawade
Summary: How I created my GitHub powered blogging webiste using pipeline for free

## Description

In this blog post, I will demonstrate the step-by-step process of creating your own static blogging website using Pelican - a static site generator and GitHub hosting in a pipeline production-deployment cycle that too for free

## Installing required software

We need to install some softwares inorder to create our pipeline, so first we will install Pelican, make sure you have Python installed
Open your Terminal in Linux or CMD in Windows & Enter following command

`python -m pip install "pelican[markdown]"`

We will also need, *git* installed, to do so 
1. In windows, follow the steps mentioned in [Git Installation guide]("https://www.atlassian.com/git/tutorials/install-git#windows") 

2. In Linux, run in terminal - `sudo apt-get install git`

## Creting GitHub repository

To create the **pipeline** we need to have a GitHub repository
1. Visit  [https://github.com/new](https://github.com/new)
2. Enter the *Repository name*
3. Click on *Create reposiroty* button to complete repository creation process

### Clone the repository locally

After the repository is created, clone it locally using command line *git* command
Example - `git clone https://github.com/<your_username>/<repository_name>`
    Replace <your_username> & <repository_name> as per your information

Go into the repository folder, using `cd <repository_name>`

## Project creation

After the base work is done, we will start creating our blogging website using **Pelican**

Enter - `pelican-quickstart` in the terminal or CMD
You will be prompted to answer few questions, related the Static site


**Step: 1**