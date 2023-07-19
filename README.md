# Thyroid Disease Detection


<img src="https://www.betterhealthclinic.ca/wp-content/uploads/2019/01/Thyroid-768x691.jpg" width="500" height="300"/>
## Problem Statement
Thyroid disease is a common cause of medical diagnosis and prediction, with an onset that is difficult to forecast in medical research. The thyroid gland is one of our body's most vital organs. Thyroid hormone releases are responsible for metabolic regulation. Hyperthyroidism and hypothyroidism are one of the two common diseases of the thyroid that releases thyroid hormones in regulating the rate of body's metabolism.

The main goal is to predict the estimated risk on a patient's chance of obtaining thyroid disease or not.

## Solution Proposed 
We need to build a ML model which will be used by hospitals and help the hospital authority to identify if the patient has thyroid or not. If it is a positive case then medical will do further test to know what type of thyroid the person is suffering from and according to that the treatment will be on fast-track.


## Approach: 
The classical machine learning tasks like Data Exploration, Data Cleaning,
Feature Engineering, Model Building and Model Testing. Try out different machine
learning algorithms that’s best fit for the above case.

## Tech Stack Used
1. Python 
2. VS Code 
3. Machine learning algorithms
4. Docker
5. MongoDB
6. Flask

## Infrastructure Required.

1. AWS S3
2. AWS EC2
3. AWS ECR
4. Github Actions
5. Airflow


## How to run?
Before we run the project, make sure that you are having MongoDB in your local system, with Compass since we are using MongoDB for data storage. You also need AWS account to access the service like S3, ECR and EC2 instances.

 







## Data Collections

![image](https://user-images.githubusercontent.com/102937478/216246951-7c187908-a8b0-4c64-8f37-6549c49e20fa.png)

## Project Archietecture

![image](https://user-images.githubusercontent.com/57321948/193536768-ae704adc-32d9-4c6c-b234-79c152f756c5.png)


## Deployment Archietecture
![image](https://user-images.githubusercontent.com/57321948/193536973-4530fe7d-5509-4609-bfd2-cd702fc82423.png)



### Step 1: Clone the repository
```bash
git clone 

### Step 2- Create a conda environment after opening the repository

```bash
conda create -n thyroid python=3.8 -y

or 

conda create --prefix ./env python=3.7 -y
conda activate ./env
```

```bash
conda activate thyroid
```

### Step 3 - Install the requirements
```bash
pip install -r requirements.txt
```

### Step 4 - Export the environment variable
```bash
export AWS_ACCESS_KEY_ID=<AWS_ACCESS_KEY_ID>

export AWS_SECRET_ACCESS_KEY=<AWS_SECRET_ACCESS_KEY>

export AWS_DEFAULT_REGION=<AWS_DEFAULT_REGION>

export MONGODB_URL="mongodb+srv://himanshu:himanshu12345@ineuron.fpig7r5.mongodb.net/?retryWrites=true&w=majority"

```

### Step 5 - Run the application server
```bash
python app.py
```


## Run locally

1. Check if the Dockerfile is available in the project directory

2. Build the Docker image
```
docker build --build-arg AWS_ACCESS_KEY_ID=<AWS_ACCESS_KEY_ID> --build-arg AWS_SECRET_ACCESS_KEY=<AWS_SECRET_ACCESS_KEY> --build-arg AWS_DEFAULT_REGION=<AWS_DEFAULT_REGION> --build-arg MONGODB_URL=<MONGODB_URL> . 

```

3. Run the Docker image
```
docker run -d -p 8080:8080 <IMAGE_NAME>
```

To run the project  first execute the below commmand.
MONGO DB URL: 
```
mongodb+srv://himanshu:himanshu12345@ineuron.fpig7r5.mongodb.net/?retryWrites=true&w=majority
```
windows user

```
mongodb+srv://himanshu:himanshu12345@ineuron.fpig7r5.mongodb.net/?retryWrites=true&w=majority
```

Linux user

```
mongodb+srv://himanshu:himanshu12345@ineuron.fpig7r5.mongodb.net/?retryWrites=true&w=majority
```

then run 
```
python main.py
```

### To download the dataset 
```
wget https://raw.githubusercontent.com/himanshubalodi62/Thyroid-Disease-Detection/main/hypothyroid.csv
```

### To check and reset git log
```
git log
git reset --soft 6afd
6afd -> last 4 digit of log. 
```

### To add and uplod to git
```
git add filename
we can also use . for all file(Current directory)

git commit -m "Message"
git push origin main
```


### **To create a new environment in vscode** 
```
 1. Select the command prompt as a terminal 
conda create -p venv python==3.87 -y
```

### Create a .env It contains details.
```
MONGO_DB_URL="mongodb://localhost:27017/neurolabDB"
AWS_ACCESS_KEY_ID="asfsdfsdgrgdfgfdgd"
AWS_SECRET_ACCESS_KEY="hsdfgdfgimsdffdgfgdfertrrg"
```
### **To install dockers in aws machine (EC2)**
```
curl -fsSL https://get.docker.com -o get-docker.sh
sudo sh get-docker.sh
sudo usermod -aG docker ubuntu
newgrp docker
```



**Secrets**
```
AWS_ACCESS_KEY_ID=
AWS_SECRET_ACCESS_KEY=
AWS_REGION=
AWS_ECR_LOGIN_URI=
ECR_REPOSITORY_NAME=
BUCKET_NAME=
MONGO_DB_URL=
```
