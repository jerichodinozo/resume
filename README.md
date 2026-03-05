# Guide to hosting your resume to a webpage
This is a guide on how to set up a webpage to display a resume.

## Purpose
This document aims to guide readers who are interested in learning more about technical writing that possess basic understanding of Markdown and the command line interface but are inexperienced with version control systems and static site generators. By the end of this guide, the reader will be able to utilize the technologies mentioned above to host static webpages that follow the guidelines from Etter's "Modern Technical Writing: An Introduction to Software Writing." This guide will be guiding the reader how to use Github, MKDocs, and Github pages to host their webpage.

## Prerequisites
- MacOS: For this guide I will be using a device with MacOS installed
- Git installed
- GitHub account
- Python installed
- Basic markdown knowledge

## Instructions

### 1. MKDocs installation
Building a website from scratch can be very tedious. Basic static webpages require knowledge of HTML, some CSS, and maybe some Javascript. Static website generators are tools that help lower the barrier of entry to building websites. In this guide, we will be using the static site generator MKDocs to generate our webpage.

#### 1.1: Open terminal
Opening terminal will allow us to install the various programs that we will be needing throughout this guide.

#### 1.2: Installing MKDocs
Once terminal is open, we will input the following command to install MKDocs:
```
python3 -m pip install mkdocs
```
Running the command above allows us to have MKDocs installed in our device.

### 2. Setting up GitHub
GitHub allows individuals to create repositories to store the files that are needed for projects. For this guide, we will need to create a repository before creating our local MKDocs project. GitHub uses Git as their version control system. Etter recommends using version control systems for projects, because they allow individuals to store documentations in the same place where the source code is, making it easier for documentations and code to stay synchronized.

#### 2.1 Create a GitHub repository
To create a GitHub repository, go to the repositories page of your profile and click "new"

#### 2.2. Select a name for the repository
Choose an easy to remember name for your repository.

#### 2.3. Create repository
Click "create repository" at the bottom of the page.

#### 2.4. Copy the  GitHub Repository link
The GitHub repository link is found here.
Copy that link.

#### 2.5. Go to terminal
Go back to terminal for the next step.

#### 2.6 Enter the following command
```
git clone <your link here>
```

### 3. Create a MKDocs Project


### 4. Create a Markdown Resume
Creating a Markdown resume is simple. For this guide, we took an existing resume and converted it to the Markdown format. Be sure to use appropriate headings and lists when it is needed.

### 5. Add Markdown Resume to Project Folder

### 6. Preview the Website
Previewing the website allows us to visualize the webpage. To preview our work so far, enter the following command in terminal.
```
python3 -m mkdocs serve
```

### 7. Deploy Project
Deploying the project to GitHub is the next step to finishing our webpage. 

### 8. Enable GitHub Pages

## Resources

## FAQ
Why is Markdown better than writing raw HTML?  

- According to Etter's "Modern Technical Writing," some markup languages like HTML tend to require individuals to write less-human readable code that is not suited for an individual that has limited technical background. Markdown is a lightweight markup language that is very simple and easy to follow.

I changed the Markdown version of my resume, so why don’t I see the changes when I refresh the website in my browser?  

- Changing the Markdown version of your resume is just one part of saving changes to your webpage. You will need to re-deploy your website on terminal to see the changes you've made.

## Credits