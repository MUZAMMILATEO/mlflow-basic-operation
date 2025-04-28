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
export MLFLOW_TRACKING_URI=https://dagshub.com/send2manoo/MLFlow-Basic-Operation.mlflow
export MLFLOW_TRACKING_USERNAME=send2manoo
export MLFLOW_TRACKING_PASSWORD=0ea83aeca6cad84965aa3308c523881447297583
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
mlflow server -h 0.0.0.0 --default-artifact-root s3://mlflow-buc23
```
Unveil your server at your EC2's Public IPv4 DNS on port 5000.

#### 🌐 Setting MLFLOW_TRACKING_URI
Craft your MLFlow tracking URI:
```bash
export MLFLOW_TRACKING_URI=http://ec2-3-80-202-174.compute-1.amazonaws.com:5000/
```

---

🌟 **Feel free to contribute!** 🌟

**Happy tracking and coding!** 🚀