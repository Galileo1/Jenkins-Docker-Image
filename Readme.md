

# To run Jenkins container
docker run -d -p 8080:8080 -p 50000:50000 -v jenkins_home:/var/jenkins_home -v /var/run/docker.sock:/var/run/docker.sock jenkins:latest

# To get the password 
docker exec ${jenkis-containerid} cat /var/jenkins_home/secrets/initialAdminPassword


