---
title: "Current Kubernetes Project"
date: 2021-11-05T14:19:52-04:00
draft: false
---
## Creating a Containerized Python Application and Deploy to Kubernetes Cluster
When JJ reached out to me regarding the job opportunity, it was a catalyst to get in gear and create a project. Docker and Kubernetes are huge pieces in the DevOps arena. I've been meaning to work on those in the near future and as I mentioned before, this opportunity is a great catalyst. This site is actually deployed via Docker and Linode's Kubernetes Engine (LKE). I will take you on a quick journey describing how, over the last 3 days, I got to this point.

### Wednesday
I've been studying Python to become more proficient with the language. I had the `learning_log` application mostly finished at the time. It just needed a bit of polish on it in terms of styling. It was completely functional. I've often wondered how to containerize and deploy applications and infrastructure and again, this was a great opportunity to work with that.  Once I got the styling of the application, next I needed to work on containerizing it. Using the web, I began my search.

The challenge I had was the Dockerfile and also choosing a web server to serve the application. I choose `gunicorn` for being highly compatible with python.  The next challenge was figuring out how to server my application with gunicorn. After scouring the web for sometime, I figured out the command by reading gunicorn's documentation and cross referencing it with other sources. Once I had the command, the Dockerfile was fairly easy to put together. I followed Docker's instructions regarding making a Dockerfile. Next challenge was how to deploy to a Kubernetes cluster.

### Thursday
I decided to create a cluster manually using `kubeadm`. I felt this would give me a more in-depth look into how Kubernetes works. I got a ton of knowledge from it. In my personal experience, when I use a tool or a process frequently, I tend to break down the individual pieces and also attempt to streamline the tool or process. As I have infrequently needed to tool with Docker or Kubernetes, I'm not proficient. However, my knowledge of Linux and my passion for solving problems, got me to a point where I had manually configured a cluster with Linode's infrastructure. It was not easy and took the better part of the day on Thursday. By dinner time I was ready to deploy the application. One small problem, I've never deployed a containerized Python application to a manually configured cluster!

Time to research. I used many of Linode's documentation and ended up deploying the container to my cluster but I was met with a "Connection Reset Error". I tore down and built up the cluster about half a dozen times trying this and trying that to get the container deployed but it did not work successfully.

### Friday
To make a long story short, I deployed this static website with Hugo and LKE to hopefully show you all I have what it takes to be on your team.  I am not done either! Over this weekend, I will be working on this to conquer this project and have my "learning_log" application be deployed over the internet.
