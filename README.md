## Jenkins Tutorial for MLOps

![Screenshot 2024-09-10 132216](https://github.com/user-attachments/assets/95dedcb5-da8b-4e7e-b0b8-bdb8ef76cd13)

![Screenshot 2024-09-10 132300](https://github.com/user-attachments/assets/9819ead5-5592-4b73-bfc2-bb61b9d5924e)

![Screenshot 2024-09-10 132326](https://github.com/user-attachments/assets/fd929d75-79d6-4abb-8569-b87b46222b60)

sudo wget -O /usr/share/keyrings/jenkins-keyring.asc \
https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key

echo "deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] https://pkg.jenkins.io/debian-stable binary/" | sudo tee /etc/apt/sources.list.d/jenkins.list > /dev/null

sudo apt-get update

sudo apt install python3 python3-pip

sudo apt-get install jenkins

http://server_ip:8080/login?from=%2F

sudo cat /var/lib/jenkins/secrets/initialAdminPassword

http://102.223.37.190:8080/safeRestart

admin b1@

sudo -u jenkins -H bash


curl -sO http://102.223.37.190:8080/jnlpJars/agent.jar & java -jar agent.jar -url http://102.223.37.190:8080/ -secret 587737172bf4ea588f4f900c55e985e6d0a6e9462dfb33ccdf029c88340c7696 -name "Dev_Agent" -webSocket -workDir "/var/lib/jenkins"