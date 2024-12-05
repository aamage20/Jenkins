##  $\color{blue} \textbf {Jenkins Installing}$
## step1: launch instance using 2 cpu and 4gb ram with 30gb storage
![image](https://github.com/user-attachments/assets/9639843c-7758-45ba-8853-457ecf1d08d5)
## step 2: connect instance to the terminal and install jenkins 
````
sudo apt update -y
sudo apt install fontconfig openjdk-17-jre -y

sudo wget -O /usr/share/keyrings/jenkins-keyring.asc \
https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key
echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \
https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
/etc/apt/sources.list.d/jenkins.list > /dev/null
sudo apt-get update -y
sudo apt-get install jenkins -y
sudo systemctl start jenkins
sudo systemctl enable jenkins
````
![image](https://github.com/user-attachments/assets/3b4af8b8-c3bc-42f5-bce0-9327d8a135cd)
## step 3: after installing jenkins copy public ip of instance and paste it in new browser with jenkins port (8080)
![image](https://github.com/user-attachments/assets/5e88df3c-c7b9-4813-87fc-d2fff8515a44)
![image](https://github.com/user-attachments/assets/6411ee32-0e3d-4da4-9d80-dabf0a31f735)
## step 4: check password of jenkins using 
````
sudo cat /var/lib/jenkins/secrets/initialAdminPassword
````
![image](https://github.com/user-attachments/assets/d31c67f5-3493-45ce-a610-83f22a62a873)
## step 5: copy password and paste it to unlock jenkins
## step 6: click on install suggested plugins
![image](https://github.com/user-attachments/assets/a1865a2b-3a42-4696-94bd-e39f7b91d79a)
## step 7: fill details and create first admin user
![image](https://github.com/user-attachments/assets/4ad09b5f-1f33-482c-a7e4-e178b9a83164)
## step 8: jenkins is ready to use
![image](https://github.com/user-attachments/assets/69193d62-868a-42fe-bb4c-af764f6f6726)






