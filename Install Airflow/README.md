# Running Airflow in Docker

P/S: Follow these steps to install the necessary tools, if you have not already done so.
   - Install Docker Community Edition (CE) on your workstation. Depending on your OS, you may need to configure Docker to use at least 4.00 GB of memory for the Airflow containers to run properly. Please refer to the Resources section in the Docker for Windows or Docker for Mac documentation for more information.
   - Install Docker Compose v1.29.1 or newer on your workstation.

1. To deploy Airflow on Docker Compose, you should fetch docker-compose.yaml. :
(curl -LfO 'https://airflow.apache.org/docs/apache-airflow/2.6.3/docker-compose.yaml')
OR
(Invoke-WebRequest -Uri 'https://airflow.apache.org/docs/apache-airflow/2.6.3/docker-compose.yaml' -OutFile 'docker-compose.yaml')

<img width="905" alt="image" src="https://github.com/SyakeerRahman/Data-Tools-Install/assets/105381652/d12e5627-671e-441d-856e-83b73ef41274">


2. Setting the right Airflow user
(mkdir -p ./dags ./logs ./plugins ./config)
OR
(New-Item -ItemType Directory -Force -Path './dags', './logs', './plugins', './config')

<img width="908" alt="image" src="https://github.com/SyakeerRahman/Data-Tools-Install/assets/105381652/9e204658-a3df-4868-8656-aff42e6a7538">


3. Create an .env file in the same folder as docker-compose.yaml
AIRFLOW_UID=50000

<img width="805" alt="image" src="https://github.com/SyakeerRahman/Data-Tools-Install/assets/105381652/f56187cd-3e3f-45a7-be8f-e7cd5af892c2">


4. Initialize the database
(docker compose up airflow-init)
 on success will show
airflow-init_1       | Upgrades done
airflow-init_1       | Admin user airflow created
airflow-init_1       | 2.6.3
start_airflow-init_1 exited with code 0


5.Running Airflow
(docker compose up) 

6. open localhost http://localhost:8080/


7. for more info can go to https://airflow.apache.org/docs/apache-airflow/stable/howto/docker-compose/index.html
     
