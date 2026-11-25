# Complaintbox

## About the Project

Complaintbox is a web-based application developed using Python and Django. It provides a platform for handling complaint-related activities through a web interface.

The project uses MySQL for database management and provides a practical example of how a Django application can be integrated into a DevSecOps workflow.

## Technologies Used

- **Python** – Programming language
- **Django** – Backend web framework
- **MySQL** – Database
- **HTML, CSS and JavaScript** – Frontend technologies
- **Docker** – Application containerization
- **Jenkins** – CI/CD automation
- **Semgrep** – Source code security scanning
- **Trivy** – Dependency vulnerability scanning
- **OWASP ZAP** – Dynamic application security testing
- **Amazon ECR** – Container image storage
- **Kubernetes (K3s)** – Application deployment
- **Argo CD** – GitOps deployment management

## Key Application Details

- Django-based web application
- Complaint-related functionality
- MySQL database integration
- Browser-based user interface

## Running the Application Locally

### 1. Clone the Repository

```bash
git clone https://github.com/Afthabahammed/Complaintbox.git
cd Complaintbox
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Configure Environment Variables

Configure the required Django and MySQL settings:

- `DJANGO_SECRET_KEY`
- `DB_NAME`
- `DB_HOST`
- `DB_USER`
- `DB_PASSWORD`
- `DB_PORT`

### 4. Apply Database Migrations

```bash
python manage.py migrate
```

### 5. Start the Application

```bash
python manage.py runserver
```

Open `http://127.0.0.1:8000` in your browser.

## DevSecOps Implementation

I integrated the application into an automated DevSecOps workflow to practice security testing, continuous integration, containerization, and deployment.

The workflow follows these steps:

1. **GitHub:** Maintains the application source code.
2. **Semgrep:** Performs Static Application Security Testing (SAST).
3. **Trivy:** Scans project dependencies for known vulnerabilities.
4. **Jenkins:** Automates the CI/CD pipeline.
5. **Docker:** Builds a container image for the application.
6. **Amazon ECR:** Stores the built Docker image.
7. **Kubernetes:** Runs the application in a containerized environment.
8. **Argo CD:** Synchronizes Kubernetes deployment configurations using GitOps.
9. **OWASP ZAP:** Performs Dynamic Application Security Testing (DAST) against the running application.

## Deployment

The application is deployed on Kubernetes using a Docker image stored in Amazon ECR.

Argo CD manages the deployment using configuration files maintained in a separate GitOps repository. This makes it easier to track and manage deployment changes.

## Project Goal

The purpose of this work was to gain hands-on experience with DevSecOps tools and understand how security scanning, Jenkins automation, Docker, AWS ECR, Kubernetes, and Argo CD work together in an application deployment workflow.
