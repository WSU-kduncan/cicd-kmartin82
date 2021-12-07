- Part 1
  - 1.) To install Docker I first used the guide at https://docs.docker.com/engine/install/ubuntu/ 
    - The first command "$ sudo apt update" ,
    - Then I installed some packages using the command  
    "$ sudo apt-get install \
    ca-certificates \
    curl \
    gnupg \
    lsb-release"   
    - Then I added the offical docker GPG key using the command "$ curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o             /usr/share/keyrings/docker-archive-keyring.gpg"  
    - Then I used the command " $ echo \
    "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu \
    $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null " 
    - This command created a stable repository for Docker
    - finally I installed docker using the command "$ sudo apt-get install docker-ce docker-ce-cli containerd.io"
  - 2.) To install and run the container image to run the web server I used the guide at https://hub.docker.com/_/httpd
    - To build the container I used the command "$ docker build -t my-apache2 ."
    - Then I ran the container using the command "$ docker run -dit --name test -p 8080:80 my-apache2" 
- Part 2 
  - 1.) I created a public repo by clicking create new repo after creating a new free account. I named the repo project_6_repo
  - 2.) Then I allowed authentication via CLI using doacker hub credentials by going to account settings -> security -> new access token
  - 3.) Next I configured github sec

- Part 3   

