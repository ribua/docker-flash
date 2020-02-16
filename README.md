
Instructions to Run the docker  container

#1 : Install the docker packages and files

yum install docker

#2: Add user to docker group

usermod -a -G docker <username>

#3. Start and Enable Docker server

systemctl enable docker.service  --now

#4. Create the docker file to create the image to be used on OS along with the requirements for it in a folder

file name Dockerfile

#5. Create image 

docker build -t flask:1 . 

# Create container using the image created 

docker run -d -p  5000:5000 flask:1  


Design decisions.
=====================

- Built from ubuntu image available on docker hub. 




