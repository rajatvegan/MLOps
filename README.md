# ON EC2 with open Public IPv4 DNS to the port 5000
sudo apt update

sudo apt install python3-pip

sudo pip3 install pipenv

sudo pip3 install virtualenv

mkdir mlflow

cd mlflow

pipenv install mlflow

pipenv install awscli

pipenv install boto3

pipenv shell

# Then set aws credentials
aws configure

# Finally
mlflow server -h 0.0.0.0 --default-artifact-root s3://<s3-bucket-name>


# ON LOCAL
aws cli installation on windows: msiexec.exe /i https://awscli.amazonaws.com/AWSCLIV2.msi   
aws configure
pip install mlflow, boto3

# set uri in your local terminal and in your code
$env:MLFLOW_TRACKING_URI="http://ec2-13-232-72-41.ap-south-1.compute.amazonaws.com:5000/" 

export MLFLOW_TRACKING_URI=http://ec2-54-147-36-34.compute-1.amazonaws.com:5000/
export MLFLOW_USERNAME=
export MLFLOW_PASSWORD=



# Chest-Cancer-Classification-using-MLflow-DVC-workflow
Update config.yaml
Update secrets.yaml [Optional]
Update params.yaml
Update the entity
Update the configuration manager in src config
Update the components
Update the pipeline
Update the main.py
Update the dvc.yaml


