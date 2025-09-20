# 🧪 AZ-104 Lab Setup Checklist  

### 1. **Azure Tenant Setup**  
- [ ] Sign up for a free Azure subscription (or use a sandbox / MSDN account).  
- [ ] Create a custom domain (e.g., `contoso.com`) and verify it in **Azure AD**.  
- [ ] Configure a naming convention for users/resources (`first.lastname`, `vm-dept-01`, etc.).  

---

### 2. **User & Group Management**  
- [ ] Import CSV of users into **Azure AD** using PowerShell / Graph.  
- [ ] Assign departments from CSV as **Azure AD attributes**.  
- [ ] Create Security Groups:  
  - `Accounting_Users`  
  - `HR_Users`  
  - `IT_Users`  
  - `Sales_Users`  
  - `Frontline_Users`  
- [ ] Add users to groups based on department.  

---

### 3. **Role-Based Access Control (RBAC)**  
- [ ] Create Resource Groups for each department.  
- [ ] Assign RBAC roles:  
  - **IT** → Contributor on IT Resource Group  
  - **Accounting / HR** → Reader (test limited access)  
  - **Sales / Frontline** → Reader or custom roles  

---

### 4. **Azure Resources**  
- [ ] Deploy a few **Virtual Machines** (Windows & Linux) in different regions.  
- [ ] Deploy a **Storage Account** for shared files.  
- [ ] Create a **Virtual Network** with subnets for testing NSGs.  
- [ ] Add a **Web App** (App Service) to test PaaS deployment.  

---

### 5. **Intune / Device Management**  
- [ ] Enroll a test Windows 10/11 VM into Intune.  
- [ ] Apply Compliance Policies (password, encryption, updates).  
- [ ] Create a Conditional Access policy (block legacy auth / require MFA).  

---

### 6. **Monitoring & Reporting**  
- [ ] Enable **Azure Monitor** and **Log Analytics Workspace**.  
- [ ] Connect VM diagnostics to Log Analytics.  
- [ ] Test Alerts (CPU usage, Sign-in anomalies).  

---

### 7. **Security & Governance**  
- [ ] Enable **MFA** for selected groups (start with IT).  
- [ ] Configure **Azure Policy** to enforce tagging and region restrictions.  
- [ ] Test **Privileged Identity Management (PIM)** if available.  

---

### 8. **Cleanup & Review**  
- [ ] Run cost analysis with **Azure Cost Management**.  
- [ ] Document what you built and practice teardown with PowerShell / CLI.  
- [ ] Rebuild to reinforce memory before the exam.  
