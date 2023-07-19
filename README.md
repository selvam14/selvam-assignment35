# hello-node

1) Created new repository in Github
   Repo Name: selvam-assignment35 (selected node for gitignore)
   
2) git clone https://github.com/selvam14/selvam-assignment35.git
   cd selvam-assignment35 on the local (Used Git Bash)
   
3) Copied the files over from 6m-cloud-3.4-cloud-native-application-containerization-i to selvam-assignment35 folder
   Files copied: .dockerignore, Dockerfile, index.js, package.json, package-lock.json\
   tested node index.js and was able to run without issues
   
4) Executed the following commands:
   git add .
   git commit -m "Push all the files"
   git push
   
5) Logged in to AWS Console > Elastic Container Registry > Create repository > selvam-assignment35

6) Opened Docker Desktop. Once opened, run the next command.

7) aws ecr get-login-password --region ap-southeast-1 | docker login --username AWS --password-stdin 255945442255.dkr.ecr.ap-southeast-1.amazonaws.com

8) docker build -t selvam-assignment35 .

9) docker tag selvam-assignment35:latest 255945442255.dkr.ecr.ap-southeast-1.amazonaws.com/selvam-assignment35:latest

10) docker push 255945442255.dkr.ecr.ap-southeast-1.amazonaws.com/selvam-assignment35:latest



