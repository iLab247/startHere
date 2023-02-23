## How to run pre-packaged teck stacks:
Quick links: List of tech stacks https://hub.docker.com/u/ilab247 
Cloud Guru offers sand boxes and cloud servers for running the above docker images (tech stacks):

1.	Create your own machine:
a.	Login to acloud.guru 
b.	Navigate to link https://learn.acloud.guru/cloud-playground/cloud-servers 
c.	Create new server – options: Distribution = Cloud Native Kubernetes, Zone =North America (or any other), Size = Large, Tag = AIML (or any other name).  Click create server.  (This will take 2-3 mins)
d.	Open terminal – username <cloud_user>, password <listed in the page>  change it to desired name (during first login)
e.	Congratulations.  You have a sandbox ready for running our tech stacks.
2.	Run our prepackaged Java tech stacks:
a.	mkdir /home/cloud_user/workspaces
b.	chmod +777 /home/cloud_user/workspaces
c.	docker run -it --network=host -v /home/cloud_user/workspaces:/workspaces ilab247/fullstack:0.01
d.	# This above will take to the root prompt
e.	su - ilab247user
f.	cd /workspaces
g.	code-server --bind-addr 0.0.0.0:8005 --auth none --user-data-dir /home/ilab247user/data --extensions-dir /home/ilab247user/extensionsCache
h.	Navigate to the URL with port mentioned to access your VS Code environment
