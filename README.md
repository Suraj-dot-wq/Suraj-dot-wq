# Hi, I'm Suraj👋

### Aspiring Cloud & DevOps Engineer | AWS | Linux | CI/CD | Infrastructure Automation

I’m a Computer Science and Design engineering student (2023–2027) focused on building practical cloud infrastructure, automating deployments, and monitoring applications.

I learn by building hands-on projects involving AWS, Linux, Docker, Terraform, Jenkins, Prometheus, and Grafana.

- ☁️ Exploring cloud infrastructure, deployment automation, and operations.
- ⚙️ Building CI/CD pipelines and containerized applications.
- 📊 Practicing infrastructure monitoring, alerting, and service recovery.
- 🎯 Looking for entry-level Cloud, DevOps, and Cloud Support opportunities.

---

## 🛠️ Technical Skills

**Cloud:** AWS EC2, VPC, Security Groups, AWS networking fundamentals

**Infrastructure as Code:** Terraform

**CI/CD & Version Control:** Jenkins, Git, GitHub, GitHub Webhooks

**Containers & Web:** Docker, Docker Compose, Nginx, Docker Hub

**Monitoring & Alerting:** Prometheus, PromQL fundamentals, Grafana, Node Exporter, Alertmanager configuration

**Operating Systems & Scripting:** Linux, Ubuntu, Python, Bash fundamentals

**Security:** Trivy container image scanning

---

## 🚀 Featured Projects

### 1. NexaVault — Multi-User Knowledge & Productivity Platform

A full-stack notes application deployed using Docker and AWS, with an automated CI/CD pipeline.

**Tech Stack:** React · Django REST Framework · MySQL · Docker · Docker Compose · Nginx · Jenkins · AWS EC2 · Docker Hub · Trivy

#### ⚙️ How the Project Works

1. **Code Development:** The application source code is maintained in GitHub, with React handling the frontend and Django REST Framework providing backend APIs.
2. **Pipeline Trigger:** When code changes are pushed to GitHub, a webhook triggers the Jenkins pipeline.
3. **Build and Scan:** Jenkins builds the Docker images and runs Trivy vulnerability scanning.
4. **Image Publishing:** The pipeline publishes the application images to Docker Hub.
5. **Deployment:** Docker Compose manages the application services on AWS EC2.
6. **Request Handling:** Nginx handles incoming web traffic and routes requests within the deployed application.
7. **Application Runtime:** The React frontend communicates with the Django backend, which uses MySQL for application data.

#### 💡 What This Demonstrates

- CI/CD automation using Jenkins and GitHub Webhooks.
- Containerization and multi-container application management.
- Docker image publishing and vulnerability scanning.
- Application deployment and web traffic handling on AWS EC2.

🔗 **Repository:** [Personal Notes App / NexaVault](https://github.com/Suraj-dot-wq/Personal-Notes-App)

---

### 2. CloudOps — Self-Healing Infrastructure Monitoring

A cloud operations project that provisions AWS infrastructure, monitors Linux resources, and attempts automatic recovery of a failed demo service.

**Tech Stack:** AWS · Terraform · Linux · Python · Prometheus · Grafana · Node Exporter · Alertmanager · systemd · Cron

#### ⚙️ How the Project Works

**Step 1 — Infrastructure Provisioning**

Terraform defines the AWS resources required for the monitoring host, including the VPC, subnet, internet gateway, routing, security group, and EC2 instance.

**Step 2 — Metrics Collection**

Node Exporter exposes Linux host metrics, including CPU, memory, and disk statistics. Prometheus scrapes these metrics at configured intervals and stores the collected time series.

**Step 3 — Visualization**

Grafana uses Prometheus as a data source. Dashboards display CPU, memory, and disk utilization so that resource usage can be inspected.

**Step 4 — Alert Evaluation**

Prometheus evaluates configured rules for high CPU, memory, and disk utilization. Alertmanager is configured for alert routing; external email or webhook delivery has not been verified.

**Step 5 — Automated Health Checks**

A Python health-check script uses system metrics to assess CPU, memory, and disk usage and writes its results to a log file. Cron schedules the script to run periodically.

**Step 6 — Service Recovery**

A separate Python self-healing script checks whether `cloudops-demo.service` is active. If the service is inactive, the script attempts to restart it through systemd using the configured permission.

**Step 7 — Recovery Verification**

The recovery workflow was tested by stopping the demo service and verifying that the script could restart it. This demonstrates basic automated service recovery rather than complete infrastructure self-healing.

#### 🔄 CloudOps Workflow

`Terraform → AWS EC2 → Node Exporter → Prometheus → Grafana`

**Independent recovery workflow:**

`Cron → Python Self-Healing Script → systemd Service Restart`

#### 💡 What This Demonstrates

- Infrastructure as Code using Terraform.
- Linux metrics collection and monitoring.
- Prometheus alert rules and Grafana dashboards.
- Python scripting, Cron scheduling, and systemd administration.
- Tested recovery of a specific demo service.

🔗 **Repository:** [CloudOps Self-Healing Monitoring](https://github.com/Suraj-dot-wq/CloudOps-Self-Healing-Monitoring)

---

## 📚 Currently Learning

- PromQL: `rate()`, `increase()`, and metric aggregation.
- AWS infrastructure troubleshooting.
- CI/CD pipeline design and deployment automation.
- Linux administration and Bash scripting.
- Cloud security, reliability, and cost optimization.





## 🎓 Education

**B.E. — Computer Science & Design**  
Atria Institute of Technology, Bengaluru  
2023–2027

**Certification:** AWS Cloud Practitioner Essential Batch— include the exact credential name and issuer that match your certificate.

---

## 🤝 Let's Connect

I'm interested in connecting with cloud engineers, DevOps professionals, recruiters, and teams working on cloud infrastructure and automation.

- **GitHub:** [Suraj-dot-wq](https://github.com/Suraj-dot-wq)
- **LinkedIn:** [Add your LinkedIn profile URL](www.linkedin.com/in/ghadage-suraj-ganpat)
- **Email:** [Add your professional email](surajghadage2004@gmail.com)

---

⭐ Thanks for visiting my profile! Feel free to explore my repositories and project implementations.
