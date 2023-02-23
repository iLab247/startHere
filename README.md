# iLab247 - the next generation lab

## Introduction

Welcome to iLab247.  iLab247 provides guidance on two major things:

1. Code repos for Research topics  
2. Tech stacks for Research & Development

You have built in tech stacks for:

- [ilab247/baseimage](https://hub.docker.com/r/ilab247/baseimage) : Ubuntu 20.04 + VSCode 
- [ilab247/javastack](https://hub.docker.com/r/ilab247/javastack) : Ubuntu 20.04 + VSCode + java + gradle
- [ilab247/fullstack](https://hub.docker.com/r/ilab247/fullstack) : Ubuntu 20.04 + VSCode + nodejs/react/angular
- [ilab247/aimlstack](https://hub.docker.com/r/ilab247/aimlstack) : Ubuntu 20.04 + VSCode + Anaconda/python/Jupyter 
- ilab247/dltstack : Ubuntu 20.04 + 

## How to run pre-packaged teck stacks:

Quick links: List of tech stacks https://hub.docker.com/u/ilab247 

Cloud Guru offers sand boxes and cloud servers for running the above docker images (tech stacks):
1.	Create your own machine:
    * Login to acloud.guru 
    * Navigate to link https://learn.acloud.guru/cloud-playground/cloud-servers 
    * Create new server – options: Distribution = Cloud Native Kubernetes, Zone =North America (or any other), Size = Large, Tag = AIML (or any other name).  Click create server.  (This will take 2-3 mins)
    * Open terminal 
        * ```– username <cloud_user>, password <listed in the page>  change it to desired name (during first login) ```
    * Congratulations.  You have a sandbox ready for running our tech stacks.
2.	Run our prepackaged Java tech stacks:
    * ```docker run -it --network=host ilab247/javastack:0.01```
    * Navigate to the URL with port mentioned to access your VS Code environment
3.	Run our prepackaged AIML tech stacks:
    * ```docker run -it --network=host ilab247/aimlstack:0.01```
    * Navigate to the URL with port mentioned to access your Jupyter environment 

