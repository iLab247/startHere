## How to run pre-packaged teck stacks:
Quick links: List of tech stacks https://hub.docker.com/u/ilab247 

Cloud Guru offers sand boxes and cloud servers for running the above docker images (tech stacks):

###### 1.	Create your own machine:

1. Login to acloud.guru 
2. Navigate to link https://learn.acloud.guru/cloud-playground/cloud-servers 
3. Create new server – options: Distribution = Cloud Native Kubernetes, Zone =North America (or any other), Size = Large, Tag = AIML (or any other name).  Click create server.  (This will take 2-3 mins)
4. Open terminal – username <cloud_user>, password <listed in the page>  change it to desired name (during first login)
5. Congratulations.  You have a sandbox ready for running our tech stacks.

###### 2.	Run our prepackaged Java tech stacks:

2. mkdir /home/cloud_user/workspaces
3. chmod +777 /home/cloud_user/workspaces
4. docker run -it --network=host -v /home/cloud_user/workspaces:/workspaces ilab247/fullstack:0.01
5. This above will take to the root prompt
6. su - ilab247user
7. cd /workspaces
8. code-server --bind-addr 0.0.0.0:8005 --auth none --user-data-dir /home/ilab247user/data --extensions-dir /home/ilab247user/extensionsCache
9. Navigate to the URL with port mentioned to access your VS Code environment
