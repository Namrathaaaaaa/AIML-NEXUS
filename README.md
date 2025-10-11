# AIML-NEXUS
# 🧠 Department Chatbot – DevOps Repository

This repository contains the **DevOps setup and workflow** for the Department Chatbot project.  
It includes CI/CD automation, branching strategy, and collaboration workflow using **GitHub, Jenkins, Docker, Kubernetes, ArgoCD, and Observability tools**.

---

## 🪴 Branching Strategy

We use a **two-branch model** for clean code flow:

| Branch | Purpose |
|---------|----------|
| **main** | Production-ready, stable code that gets deployed to the `prod` namespace in Kubernetes. |
| **preprod** | Testing and staging branch where new features are integrated and validated before moving to `main`. |

All developers work on **feature branches**, test them, and then raise a **Pull Request (PR)** to merge into `preprod`.

---

## 🔀 Contribution Workflow

Follow these steps to **fork and contribute** to this project:

### 1️⃣ Fork the Repository
Click the **“Fork”** button (top right of this page) to create your own copy under your GitHub account.

### 2️⃣ Clone Your Fork
```bash
git clone https://github.com/<your-username>/department-chatbot-devops.git

