# Installing Superset Locally Using Docker Compose

 1. Install a Docker Engine and Docker Compose 
(https://docs.docker.com/desktop/install/windows-install/)

2. Clone Superset's GitHub repository
Clone Superset's repo in your terminal with the following command:

(git clone https://github.com/apache/superset.git)

Once that command completes successfully, you should see a new superset folder in your current directory.

3. Launch Superset Through Docker Compose
Navigate to the folder you created in step 1:

(cd superset)

When working on master branch, run the following commands:

(docker-compose -f docker-compose-non-dev.yml pull)
(docker-compose -f docker-compose-non-dev.yml up)

4. Log in to Superset
You can access Superset now via your web browser by visiting (http://localhost:8088)
username: admin
password: admin

<img width="930" alt="image" src="https://github.com/SyakeerRahman/Data-Tools-Install/assets/105381652/7f6fd346-3f24-4b6b-a5d4-a023f79d374d">
