sudo apt update
sudo apt upgrade -y
sudo apt install -y openjdk-17-jdk
java --version
![image](https://github.com/user-attachments/assets/6ed17dd0-d0dd-42c0-a21e-407acb1cb2a9)

Install and configure PostgreSQL
sudo sh -c 'echo "deb http://apt.postgresql.org/pub/repos/apt/ `lsb_release -cs`-pgdg main" /etc/apt/sources.list.d/pgdg.list'
![image](https://github.com/user-attachments/assets/1f97e4ae-c98f-421b-8ccd-f5499142242f)

wget -q https://www.postgresql.org/media/keys/ACCC4CF8.asc -O - | sudo apt-key add -

![image](https://github.com/user-attachments/assets/e248bf24-9eb0-4e7e-97d6-cec490a916e0)

![image](https://github.com/user-attachments/assets/3abf0b88-1acf-4562-bcbc-ea33fa74dee8)

sudo systemctl enable postgresql
sudo systemctl start postgresql
sudo systemctl status postgresql

![image](https://github.com/user-attachments/assets/334afc41-a4e3-4fb9-a167-054cb3d17732)

psql --version
![image](https://github.com/user-attachments/assets/237c0dcb-8e33-4f19-b927-fc749bd679a7)

sudo -i -u postgres

createuser ddsonar
psql
ALTER USER ddsonar WITH ENCRYPTED password 'nikita0919';
CREATE DATABASE ddsonarqube OWNER ddsonar;
GRANT ALL PRIVILEGES ON DATABASE ddsonarqube to ddsonar;

![image](https://github.com/user-attachments/assets/95c503c1-c549-427f-b600-18398828cb76)
\l

![image](https://github.com/user-attachments/assets/cddffae4-66b0-45a1-940d-f837dfbb2830)

\du
\q

5) Download and Install SonarQube

   

![image](https://github.com/user-attachments/assets/24861436-d547-4029-b764-9db830e576c2)

sudo apt install zip -y
sudo wget https://binaries.sonarsource.com/Distribution/sonarqube/sonarqube-10.0.0.68432.zip

![image](https://github.com/user-attachments/assets/e5bc5165-8630-472f-a7fa-cdc6ef53b59d)

![image](https://github.com/user-attachments/assets/c5ba81d8-99c6-4a68-95c7-ff70df9c98e3)

![image](https://github.com/user-attachments/assets/2c08a986-33c7-45e9-8c72-eee181c8cf4d)

![image](https://github.com/user-attachments/assets/b7849875-8656-456d-a13f-fdbe201129c5)




