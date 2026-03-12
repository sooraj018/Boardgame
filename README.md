# BoardgameListingWebApp

## Description 

**Board Game Database Full-Stack Web Application.**
This web application displays lists of board games and their reviews. While anyone can view the board game lists and reviews, they are required to log in to add/ edit the board games and their reviews. The 'users' have the authority to add board games to the list and add reviews, and the 'managers' have the authority to edit/ delete the reviews on top of the authorities of users.  

# 🚀 End-to-End DevSecOps Pipeline: Java Boardgame App

[![Jenkins](https://img.shields.io)](https://www.jenkins.io)
[![Kubernetes](https://img.shields.io)](https://kubernetes.io)
[![Docker](https://img.shields.io)](https://www.docker.com)
[![Security](https://img.shields.io)](https://aquasecurity.github.io)

## 📖 Project Overview
This repository contains a fully automated, **security-focused CI/CD pipeline** for a Java-based Boardgame application. The project bridges the gap between Development, Security, and Operations by implementing "Security Left" principles and full-stack observability.

---

## 🏗️ Architecture Highlights

### 🔹 Infrastructure & Orchestration
*   **Cloud:** Provisioned on **AWS EC2**.
*   **Cluster:** Self-managed **Kubernetes Cluster** (Control Plane + Worker Nodes) configured via `Kubeadm`.
*   **CI/CD:** Orchestrated using **Jenkins Declarative Pipelines**.

### 🔹 The Pipeline Stages
1.  **Build & Test:** Automated compilation using **Maven** and **JDK 17**.
2.  **Static Analysis:** **SonarQube** integration with mandatory Quality Gates.
3.  **Vulnerability Scanning:** **Trivy** scans for both the File System and Docker Images.
4.  **Artifact Management:** Build artifacts published to **Nexus Repository Manager**.
5.  **Containerization:** Optimized **Docker** image creation and push to Docker Hub.
6.  **Deployment:** Automated deployment to the K8s cluster with post-deployment verification.

### 🔹 Observability Stack
*   **Metrics:** **Prometheus** & **Grafana** for real-time resource tracking.
*   **Node Monitoring:** **Node Exporter** for server-level health.
*   **Uptime:** **Blackbox Exporter** for endpoint probing and availability.

---

## 💡 Key Lessons Learned
*   **Troubleshooting:** Resolved complex `CrashLoopBackOff` errors and API version mismatches in Kubernetes.
*   **DevSecOps:** Implemented automated security gating to prevent vulnerable images from reaching production.
*   **Integration:** Mastered the webhook and authentication flow between Jenkins, K8s, and monitoring tools.

---

## 🛠️ Tech Stack

| Category | Tools |
| :--- | :--- |
| **CI/CD** | Jenkins, Maven |
| **Cloud/K8s** | AWS, Kubeadm, Kubernetes |
| **Security** | SonarQube, Trivy |
| **Registry** | Docker Hub, Nexus |
| **Monitoring** | Prometheus, Grafana, Blackbox Exporter |

---

## 🔗 Connect with Me
Interested in DevOps or have questions about this pipeline?
*   **LinkedIn:** www.linkedin.com/in/sooraj-chandran-8893b6252

## Technologies

- Java
- Spring Boot
- Amazon Web Services(AWS) EC2
- Thymeleaf
- Thymeleaf Fragments
- HTML5
- CSS
- JavaScript
- Spring MVC
- JDBC
- H2 Database Engine (In-memory)
- JUnit test framework
- Spring Security
- Twitter Bootstrap
- Maven

## Features

- Full-Stack Application
- UI components created with Thymeleaf and styled with Twitter Bootstrap
- Authentication and authorization using Spring Security
  - Authentication by allowing the users to authenticate with a username and password
  - Authorization by granting different permissions based on the roles (non-members, users, and managers)
- Different roles (non-members, users, and managers) with varying levels of permissions
  - Non-members only can see the boardgame lists and reviews
  - Users can add board games and write reviews
  - Managers can edit and delete the reviews
- Deployed the application on AWS EC2
- JUnit test framework for unit testing
- Spring MVC best practices to segregate views, controllers, and database packages
- JDBC for database connectivity and interaction
- CRUD (Create, Read, Update, Delete) operations for managing data in the database
- Schema.sql file to customize the schema and input initial data
- Thymeleaf Fragments to reduce redundancy of repeating HTML elements (head, footer, navigation)

## How to Run

1. Clone the repository
2. Open the project in your IDE of choice
3. Run the application
4. To use initial user data, use the following credentials.
  - username: bugs    |     password: bunny (user role)
  - username: daffy   |     password: duck  (manager role)
5. You can also sign-up as a new user and customize your role to play with the application! 😊
