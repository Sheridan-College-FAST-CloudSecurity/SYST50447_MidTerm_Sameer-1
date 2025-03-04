# MidTerm Exam: Secure CI/CD Workflow with GitHub Actions and Cloud Integration

You have been hired by a small business to help implement **DevOps and Security best practices** for deploying their web application. Currently, the organization lacks proper automation and security measures. Below are the **key issues** with their current workflow:

- The web application is **not stored in any source control system (SCM)**.
- **Build and deployment processes are manual**, leading to inconsistencies.
- **Code changes are deployed immediately** without any review.
- **No testing or security scanning** is performed before deployment.

Your **task** is to improve their **CI/CD pipeline**, introduce **testing and security scanning**, and set up **GitHub Actions for automation** using the provided Flask application.

---

## **1. Suggest Improvements for Development, CI, Testing, and Security Scanning**

To improve the workflow, map the **current gaps** to **proposed solutions and relevant tools**.  
Use the format below:

| Problem                                    | Solution                                      | Tool(s)          |
|--------------------------------------------|-----------------------------------------------|------------------|
| The code is not in SCM                     | Store the application code in SCM            | GitHub          |

---

## **2. Setting Up a GitHub Repository for the Application**

Follow these steps to set up your repository:

1. **Create a private repository**  
   - Name it: `SYST50447_MidTerm_[student name]`  
   - Create it in the `Sheridan-College-FAST-CloudSecurity` GitHub organization.  

2. **Enable branch protection for the main branch**  
   - Restrict direct pushes to `main`.  
   - Require **pull requests (PRs)** for changes.  

---

## **3. Configure Codespaces for GitHub Repository**

1. **Set up permissions** to allow working with a remote GitHub repository.  
2. **Clone the new repository into Codespaces**.  
3. **Create a new branch named `midterm`**.  
4. **Add the provided application and unit test files** to this branch.  
5. **Verify the application works in the CodeSpaces environnment by executing the provided unit test**
6. **Commit and push** all changes to the remote repository (`midterm` branch).  

---

## **4. Add a GitHub Actions Workflow**

Create a **CI/CD workflow** using GitHub Actions:  

1. **Create a YAML file for automation**  
   - Save it as `.github/workflows/ci.yml`.  

2. **Define workflow triggers**  
   - Run on **every Pull Request (PR) or push to the main branch**.
   - Use Python version 3.12

3. **Automate the following steps**  
   - **Install dependencies** from `requirements.txt`.  
   - **Perform API endpoint testing** for:
     - `GET /health`  

---

## **5. Submission Requirements**

### **Deliverables:**

- A **private GitHub repository link** containing all your work.
- A **Word or PDF document** that includes:
  - Screenshots for each step.
  - **Captions explaining** what the screenshot demonstrates.

Grading Criteria

| Task                                         | Points |
|----------------------------------------------|--------|
| Suggested changes                            | 10     |
| GitHub repo and branch Protection Rules      | 10     |
| Setting up local git environment and pushing code to the remote repo | 10     |
| CI Workflow Implementation                   | 20     |
| **Total**                                    | 50     |
