# 🚀 MLFlow-Basic-Operation

**Welcome to MLFlow-Basic-Operation!** Dive into the world of MLFlow, your go-to platform for tracking and managing machine learning experiments.

---

## 📚 Documentation & Tutorials
- [📘 Official Documentation](https://mlflow.org/docs/latest/index.html)

---

## 🛠️ Getting Started
Ready to embark on your MLFlow journey? Launch the MLflow UI with ease:
```bash
mlflow ui
```

---

### 🌐 Integration with Dagshub
Seamlessly integrate MLFlow with Dagshub for collaborative tracking.
```bash
set MLFLOW_TRACKING_URI=https://dagshub.com/MUZAMMILATEO/<REPOSITORY_NAME>.mlflow
set MLFLOW_TRACKING_USERNAME=<YOUR_MLFLOW_TRACKING_USERNAME>
set MLFLOW_TRACKING_PASSWORD=<YOUR_MLFLOW_TRACKING_PASSWORD>
```
Execute these commands to configure your environment.

---

### ☁️ MLFlow on AWS
Elevate your MLFlow experience on AWS:

#### 🚀 Setup
- **AWS Console:** Log in and navigate to glory.
- **IAM User:** Craft with AdministratorAccess.
- **AWS CLI:** Set sail with `bash aws configure `.
- **S3 Bucket:** Create your data treasure chest.
- **EC2 Instance:** Launch Ubuntu and fortify with Security Groups for port 5000.

#### 🛠️ Installation & Configuration
```bash
sudo apt update
sudo apt install python3-pip
sudo pip3 install pipenv virtualenv

mkdir mlflow && cd mlflow
pipenv install mlflow awscli boto3
pipenv shell
```
Arm yourself with AWS credentials using \`bash aws configure \`.

#### 🚀 Running MLflow Server
```bash
mlflow server -h 0.0.0.0 --default-artifact-root s3://<BUCKET_NAME?
```
Unveil your server at your EC2's Public IPv4 DNS on port 5000.

#### 🌐 Setting MLFLOW_TRACKING_URI
Craft your MLFlow tracking URI:
```bash
export MLFLOW_TRACKING_URI=http://ec2-00-00-00-00.eu-north-1.compute.amazonaws.com:5000/
```

---

🌟 **Feel free to contribute!** 🌟

**Happy tracking and coding!** 🚀