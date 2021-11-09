---
title: "Monday Evening"
date: 2021-11-09T08:25:23-05:00
draft: false
---
## Called in for Support
The weather is nice and I did some bodywork on my 1982 Volvo wagon. This evening though, I sat down and continued my journey learning how to deploy my python application.  I've been creating different clusters in different ways. The three ways I've been using are:

1. [`kubeadm` with my Ansible playbooks](https://www.linode.com/docs/guides/getting-started-with-kubernetes/)
2. [Using Linode Kubernetes Engine (LKE)](https://www.linode.com/docs/guides/how-to-deploy-a-static-site-on-linode-kubernetes-engine/)
3. [Using Azure Kubernetes Service (AKS)](https://docs.microsoft.com/en-us/azure/aks/tutorial-kubernetes-prepare-app)

After I get the cluster running, I then deploy the test application; which works! I then deploy my application, in a similar manner and have not yet met success. However, this journey has been littered with golden nuggets of knowledge.

Last night was the first time I deployed Azure's Kubernetes offering. I was able to run their application through [their tutorial.](https://docs.microsoft.com/en-us/azure/aks/tutorial-kubernetes-prepare-app) But again when I tried my application, it did not launch.  So I went to `r/devops` on reddit and asked [this question of the community.](https://www.reddit.com/r/devops/comments/qpsfj1/just_putting_this_out_there_for_now_asking_for/)

I received great feedback and will use it to work on this further.  Each day I feel this is the day the python app will be deployed. Today is no different.
