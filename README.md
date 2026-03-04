# Guide to hosting your resume to a webpage
This is a guide on how to set up a webpage to display a resume.

## Purpose
This guide aims to help those who are new to building webpages to deploy their first project. This guide will display a resume to a webpage. We will be using Markdown to lay the resume details out, Github to host our webpage files, and MKdocs to build a static website.

## Prerequisites
- MacOS
- Git installed
- Github account
- Python installed
- basic markdown knowledge

## Instructions

### MKDocs installation
Building a website from scratch can be very tedious. Basic static webpages require knowledge of HTML, some CSS, and maybe some Javascript. Static website generators are tools that help lower the barrier of entry to building websites. In this guide, we will be using the static site generator MKDocs to generate our webpage.

#### Step 1: 

# FAQ
- When I login to github on terminal, I encounter invalid username or password, how do I fix this?
This happens when you have 2FA enabled on your account. You will need to generate a token and input that token with your password when you log in.

- When I tried installing Jekyll, I got an error, what do I do?
No big deal! Try updating your Ruby version then try installing Jekyll again.

# Steps I've done
I first created a resume using stackedit (a markdown editor). 
Then I uploaded that resume md file to github.

I did, 
```
git commit
git push origin
```

```
python3 -m pip install mkdocs
```