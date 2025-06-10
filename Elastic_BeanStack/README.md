# AWS Elastic Beanstalk Node.js Application

This project demonstrates how to deploy a simple **Node.js application** using **AWS Elastic Beanstalk**.

📦 **GitHub Repo**: [AnushreeGM/nodejsapp](https://github.com/AnushreeGM/nodejsapp.git)

---

## 🌱 What is AWS Elastic Beanstalk?

**AWS Elastic Beanstalk** is a Platform as a Service (PaaS) offered by AWS. It allows developers to easily deploy and manage applications in the cloud without worrying about the underlying infrastructure.

### 🚀 Features:
- Automatically handles capacity provisioning, load balancing, scaling, and health monitoring.
- Supports multiple programming languages and platforms including Node.js, Python, Java, .NET, PHP, Ruby, and Go.
- Full control of AWS resources via environment configuration.

---

## 📁 Project Structure

```
nodejsapp/
├── index.html         # Sample HTML page for Elastic Beanstalk welcome page
├── app.js             # Node.js entry point (if used)
├── package.json       # Defines dependencies
├── .ebextensions/     # (Optional) EB configuration folder
```

---

## 🛠️ Step-by-Step: Deploy to Elastic Beanstalk

### Step 1: Install AWS CLI and EB CLI

```bash
pip install awsebcli --upgrade
aws configure
```

> Provide your AWS Access Key, Secret, Region (e.g. `us-east-1`), and Output format.

---

### Step 2: Clone the GitHub Repo

```bash
git clone https://github.com/AnushreeGM/nodejsapp.git
cd nodejsapp
```

---

### Step 3: Initialize Elastic Beanstalk Project

```bash
eb init
```

- Choose your AWS region.
- Select **Node.js** as the platform.
- Answer prompts for SSH key setup if needed.

---

### Step 4: Create and Deploy Environment

```bash
eb create my-node-env
```

This command:
- Provisions an environment.
- Deploys your code.
- Sets up EC2, S3, CloudWatch, Load Balancer automatically.

---

### Step 5: Open Your Application

```bash
eb open
```

This opens the public URL of your Beanstalk app in the browser.

---

## 🧹 To Clean Up (Delete Resources)

```bash
eb terminate my-node-env
```

This deletes the environment and associated AWS resources.

---

## 🔗 Useful Links

- [AWS Elastic Beanstalk Documentation](https://docs.aws.amazon.com/elasticbeanstalk/latest/dg/Welcome.html)
- [Beanstalk Node.js Platform Info](https://docs.aws.amazon.com/elasticbeanstalk/latest/dg/create_deploy_nodejs.html)
- [GitHub Repo](https://github.com/AnushreeGM/nodejsapp.git)

---

## 👩‍💻 Author

**Anushree GM**

---

## 📜 License

This project is licensed under the MIT License.
