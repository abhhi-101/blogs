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
Open your Terminal in Linux or  CMD in Windows & Enter following command

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
**Step: 1** - Creating project using Pelican

Enter in the terminal or CMD
> pelican-quickstart

You will be prompted to answer few questions, related the Static site

`Where do you want to create your new web site?`
> .
 
`What will be the title of this web site?`
> mypersonalblogs

`Who will be the author of this web site?`
> Abhishek

`What will be the defauly language of this web site?`
> en

`Do you want to specify a URL perfix?`
> n

`Do you want to enable article pagination?`
> Y

`How many articles per page do you want?`
> 10

`What is your time zone?`
> 

`Do you want to generate a tasks.py?`
> n

**Step: 2** - Creating our first blog
2 Folders named - Content, Output & 4 Python files will be created

Now we will start creating blogs, 
1. Create a new folder inside `content` folder names `pages`
This will be the folder where we will store all our **markdown** files with `.md` extension

2. Inside the `pages` folder, create a file named `firstblog.md`
Now, we can write our first blog in `firstblog.md` file

Enter the following text in `firstblog.md` file
```
Title: First blog via Pipeline
Date: 2023-01-22 10:20
Category: Personal Blogs
Slug: first-blog
Authors: Abhishek Birdawade
Summary: Creating my first blog via Pipeline using Pelican 

## My first day in School
I was very excited yet nervous during my first day in school. I woke up early before my alarm and my mom helped me to get ready.

Mom packed **Pasta** in my tiffin box, which I ate during the recess time.

We were taught about a quote, stating 
> It's not what happens to you, but how you react to it that matters.

I made many new friends and played with them, finally at evening time, I came back home in our school bus.
```

**Step: 3** - Generating .html file from .md file
Now that we have created our first blog in `.md` file, we will convert it into `.html` file using Pelican

> pelican -s .\pelicanconf.py -o .

This will create `firstblog.html` file in our working directory


**Step: 4** - uploading to GitHub
Now we are ready with our desire file, we can upload all the files to GitHub using `git` command

To add files 
> git add .

To commit changes in the branch
> git commit -m "Created our first blog"

To push to main branch in GitHub
> git push

You will see that all the files are pushed to GitHub and by repeating **Step 2.2, 3, & 4** you can create a **Pipeline structure**

**Step: 5** - Hosting using GitHub for free
Now that all our files are ready and we can host our blogging website, we will use GitHub free hosting. To do so, 

1. Go to `Setting` of your GitHub Repository
2. From left side panel, select `Pages` setting
3. Under `Branch` section, change the settings from `None` to `main` & Click `Save`

Your website is now public and anyone across the web can access & read your blogs at https://<your_username>.github.io/<github_repository_name>

--- 

That was all, hope you liked the blog, Thanks for visiting :)
