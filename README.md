### Link to Docker hub repository: https://hub.docker.com/repository/docker/rolakeanney/mynginximage

### Steps I toook to create and test the Dockerfile
- I created an empty file in the folder of my choice named Dockerfile
- I created an HTML file containing the text, 'Welcome to SCA Cloud School Application'
- On my terminal, after changing directory to the folder in use, I ran the 'vim Dockerfile' command to enable me add the instructions to my Dockerfile. The content of the file can be seen in the repository
- After that, I exited the Dockerfile and ran the command 'docker build -t myimagename .' to build the image
- Then I ran the command 'docker run -p 80:80 --name=dev2 mynginximage', to run the image and check if the webpage is displayed on my localhost with the specified port number (80). 

### Steps for deployment
 To push my image to dockerhub, I ran the following commands
 - docker login: to login to dockerhub via the terminal
 - docker tag mynginximage:latest rolakeanney/mynginximage: to tag the image
 - docker push rolakeanney/mynginximage: to push to dockerhub
