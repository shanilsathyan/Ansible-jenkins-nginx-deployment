# 🚀 Automated Nginx Deployment with Ansible & Jenkins CI/CD

This project demonstrates **end-to-end automation** of Nginx web server deployment using **Ansible** and **Jenkins**.

It automates:
- Installation of Nginx on remote Linux servers.
- Configuration of a custom dynamic landing page.
- CI/CD pipeline integration with Jenkins for automated deployments.

---

## 📋 Project Overview
This project automates:
1. Nginx installation & setup on remote target servers.
2. Dynamic deployment of a web page via Ansible Templates.
3. Efficient service management using Ansible Handlers.
4. Integration with Jenkins for Continuous Deployment.

---

## ⚙️ Tools & Technologies
| Tool       | Purpose                              |
|------------|--------------------------------------|
| Ansible    | Configuration Management & Automation |
| Jenkins    | Continuous Integration & Delivery     |
| SSH        | Secure Remote Server Access           |
| Nginx      | Web Server (Deployment Target)        |
| Jinja2     | Template Engine for Dynamic Configs   |

---

## 📂 Project Structure
ansible-deploy-nginx/

│
├── inventory # Ansible Inventory File
├── nginx.yml # Main Playbook (Triggers Role)
│
└── nginx_role/ # Ansible Role (Modular Structure)
├── tasks/
│ └── main.yml # Nginx Installation & Config
├── handlers/
│ └── main.yml # Handler to Restart Nginx
├── templates/
│ └── index.html.j2 # Dynamic Landing Page Template
├── defaults/
│ └── main.yml # Default Variables


---

## 🚀 CI/CD Workflow
1. Jenkins job pulls Ansible project.
2. Jenkins runs the Ansible playbook:
   - Connects to target server using SSH key.
   - Deploys Nginx & customized landing page automatically.
3. Nginx is automatically restarted (only when config changes).

---

## 🔥 Key Features
- SSH Key-Based Automation.
- Idempotent Nginx Installation (Safe Re-runs).
- Dynamic Web Page Deployment using Jinja2 Templates.
- Ansible Handlers for Efficient Restarts.
- Full CI/CD Pipeline with Jenkins + Ansible.

---

## 🏗️ How to Run Locally
1. Configure your Ansible `inventory` file with target server(s).
2. Ensure SSH keys are properly set up.
3. Run manually:
bash
ansible-playbook nginx.yml
Or via Jenkins pipeline:
cd /path/to/project
ansible-playbook nginx.yml


## Real-World Skills Practiced
1. Infrastructure as Code (IaC)
2. Configuration Management (Ansible)
3. Continuous Integration & Delivery (Jenkins)
4. SSH & Linux Server Automation
5. Ansible Roles, Variables, Templates, Handlers

Automation Pipeline Design

👨‍💻 Author
Shanil Sathyan


## ✅ Next Step (Important!):
1. Replace this with your GitHub username:
```bash
[GitHub Profile](https://github.com/your-github-username)
