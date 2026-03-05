# Guide to hosting your resume to a webpage
This is a guide on how to set up a webpage to display a resume.

## Table of Contents

1. [Purpose](#purpose)
2. [Prerequisites](#prerequisites)
3. [Instructions](#instructions)
   - [1. MkDocs Installation](#1-mkdocs-installation)
   - [2. Setting up GitHub](#2-setting-up-github)
   - [3. Create a MkDocs Project](#3-create-a-mkdocs-project)
   - [4. Create a Markdown Resume](#4-create-a-markdown-resume)
   - [5. Add Markdown Resume to Project Folder](#5-add-markdown-resume-to-project-folder)
   - [6. Preview the Website](#6-preview-the-website)
   - [7. Push your files to GitHub](#7-push-your-files-to-github)
   - [8. Deploy MkDocs project](#8-deploy-mkdocs-project)
   - [9. Enable GitHub Pages](#9-enable-github-pages)
4. [Resources](#resources)
5. [FAQ](#faq)
6. [Credits](#credits)

## Purpose
This document aims to guide readers who are interested in learning more about technical writing that possess basic understanding of Markdown and the command line interface but are inexperienced with version control systems and static site generators. By the end of this guide, the reader will be able to utilize the technologies mentioned above to host static webpages that follow the guidelines from Etter's "Modern Technical Writing: An Introduction to Software Writing." This guide will be guiding the reader how to use Github, MkDocs, and Github pages to host their webpage.

## Prerequisites
- MacOS: For this guide I will be using a device with MacOS installed
- Git installed
- GitHub account
- Python installed
- Basic markdown knowledge

## Instructions

### 1. MkDocs installation
Building a website from scratch can be very tedious. Basic static webpages require knowledge of HTML, some CSS, and maybe some Javascript. Static website generators are tools that help lower the barrier of entry to building websites. In this guide, we will be using the static site generator MkDocs to generate our webpage.

#### 1.1: Open terminal
Opening terminal will allow us to install the various programs that we will be needing throughout this guide.

#### 1.2: Installing MkDocs
Once terminal is open, we will input the following command to install MkDocs:
```
python3 -m pip install mkdocs
```
Running the command above allows us to have MkDocs installed in our device.

### 2. Setting up GitHub
GitHub allows individuals to create repositories to store the files that are needed for projects. For this guide, we will need to create a repository before creating our local MkDocs project. GitHub uses Git as their version control system. Etter recommends using version control systems for projects, because they allow individuals to store documentations in the same place where the source code is, making it easier for documentations and code to stay synchronized.

#### 2.1 Create a GitHub repository
To create a GitHub repository, go to the repositories page of your profile and click "new"

#### 2.2. Select a name for the repository
Choose an easy to remember name for your repository.

#### 2.3. Finish creating a repository
Click "create repository" at the bottom of the page to finish up the setup of your first GitHub repository.

#### 2.4. Copy the  GitHub Repository link
The GitHub repository link is found here.
Copy that link.

#### 2.5. Go to terminal
Go back to terminal for the next step.

#### 2.6 Enter the following command
```
git clone <your link here>
```

### 3. Create a MkDocs Project
To create an MkDocs project, we use the following command on the terminal while being on the directory of your preference.
```
python3 -m mkdocs new <title of your project>
```


### 4. Create a Markdown Resume
Creating a Markdown resume is simple. For this guide, we took an existing resume and converted it to the Markdown format. Be sure to use appropriate headings and lists when it is needed.

#### 4.1. Save Markdown Resume
Save your markdown resume and name it as "index.md"

### 5. Add Markdown Resume to Project Folder
Add your markdown resume to the project folder, specifically in the following directory
```
docs
├─── index.md // replace the existing index.md with your resume
```
### 6. Preview the Website
Previewing the website allows us to visualize the webpage. To preview our work so far, enter the following command in terminal.
```
python3 -m mkdocs serve
```

### 7. Push your files to GitHub
Pushing your files to GitHub means saving the files from your local repository to the online repository. To push your files to GitHub, you will need to do the following:
#### 7.1 Choose the files you want to push to GitHub
You will need to specify what files you have modified and would like to be pushed on to the online repository, to do that, run the following command
```
git add index.md
```

#### 7.2 Commit changes
After adding the files modified, you must commit your changes to GitHub and choose an appropriate message that describes the changes you've made.
```
git commit -m "added resume file"
```

#### 7.3 Push to origin
Pushing to origin means to push your changes onto the online repository, this means that the changes you've made will be visible in the online repository.
```
git push origin
```

### 8. Deploy MkDocs project
Deploying MkDocs project allows MkDocs to generate a static website using the index.md file that you have in the docs folder. To deploy, run the command below in terminal
```
python3 -m mkdocs gh-deploy
```
Running this command allows MkDocs to automatically create a gh-page branch and push them to GitHub.

### 9. Enable GitHub Pages

## Resources
- [commonmark.org](https://commonmark.org/help/tutorial/) is a great interactive learning tool for beginners learning Markdown. This resource allows individuals to learn about Markdown by performing hands-on tasks while introducing the Markdown syntax.

- [GitHub Pages documentation](https://docs.github.com/en/pages) is a great resource for learning more about GitHub pages. There are articles that inform readers the capabilities and features of GitHub pages.

- [MkDocs User Guide](https://www.MkDocs.org/user-guide/) provides documentation on how to setup MkDocs and showcases how to use the various features of MkDocs.

- [Modern Technical Writing: An Introduction to Software Documentation](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS) is the book this documentation is modeled on. This book provides guidelines on how write technical documents.

## FAQ
### Why is Markdown better than writing raw HTML?  

- According to Etter's "Modern Technical Writing," some markup languages like HTML tend to require individuals to write less-human readable code that is not suited for an individual that has limited technical background. Markdown is a lightweight markup language that is very simple and easy to follow.

### I changed the Markdown version of my resume, so why don’t I see the changes when I refresh the website in my browser?  

- Changing the Markdown version of your resume is just one part of saving changes to your webpage. You will need to re-deploy your website on terminal to see the changes you've made.

## Credits