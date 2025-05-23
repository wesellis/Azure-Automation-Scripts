# Azure Automation Scripts - Complete Professional Toolkit

**Author**: Wesley Ellis  
**Email**: wes@wesellis.com  
**Website**: wesellis.com  
**Created**: May 23, 2025  
**Updated**: May 23, 2025 (v5.0 - Identity & Governance Enhanced)

## Overview

This collection contains **112 professionally enhanced Azure automation scripts** organized into **6 logical folders**. This represents the most comprehensive Azure automation toolkit available, with **complete Identity & Governance coverage** for enterprise security and compliance.

## 🎯 **What Makes This Collection Special**

- ✅ **112 Professional Scripts** - Complete Azure coverage including advanced identity
- ✅ **Professional Headers** with author information and contact details
- ✅ **Enhanced Functionality** beyond basic Azure commands
- ✅ **Consistent Naming Convention** (`Azure-[Service]-[Action]-Tool.ps1`)
- ✅ **Comprehensive Error Handling** and user-friendly output
- ✅ **Security Best Practices** built into each script
- ✅ **Complete Identity & Governance** - Enterprise-grade security tools

## 📁 **Complete Folder Organization - 112 Scripts**

### **👥 Identity-Governance** (12 scripts) ⭐ **ENHANCED**
*Complete Identity Management, Security, and Compliance Suite*

#### Core Identity Management (5 scripts)
- `Azure-Bulk-User-Offboarding-Tool.ps1` - Automated user offboarding
- `Azure-ServicePrincipal-Creator.ps1` - ⭐ **NEW** - Creates service principals for automation
- `Azure-AD-Group-Creator.ps1` - ⭐ **NEW** - Creates Azure AD groups with members
- `Azure-ManagedIdentity-Creator.ps1` - ⭐ **NEW** - Creates managed identities
- `Azure-Custom-Role-Creator.ps1` - ⭐ **NEW** - Creates custom RBAC roles

#### Access Management & Security (4 scripts)
- `Azure-Role-Assignment-Manager.ps1` - ⭐ **NEW** - Manages role assignments
- `Azure-PIM-Role-Activator.ps1` - ⭐ **NEW** - Activates privileged identity roles
- `Azure-ConditionalAccess-Policy-Creator.ps1` - ⭐ **NEW** - Creates conditional access policies
- `Azure-Access-Review-Creator.ps1` - ⭐ **NEW** - Creates access reviews for compliance

#### Governance & Compliance (3 scripts)
- `Azure-Policy-Assignment-Creator.ps1` - Creates policy assignments
- `Azure-ResourceGroup-Creator.ps1` - Creates resource groups with tags
- `Azure-Subscription-Security-Auditor.ps1` - ⭐ **NEW** - Comprehensive security audit

### **🖥️ Compute-Management** (31 scripts)
*Virtual Machines, Containers, Kubernetes, and Compute Resources*

[Previous content unchanged - 31 scripts including VM management, containers, etc.]

### **🌐 Network-Security** (19 scripts)
*Networking, Load Balancing, DNS, Security Infrastructure*

[Previous content unchanged - 19 scripts including networking, VPN, security, etc.]

### **💾 Data-Storage** (15 scripts)
*Databases, Storage Accounts, Data Analytics, Caching*

[Previous content unchanged - 15 scripts including storage, databases, etc.]

### **🚀 App-Development** (14 scripts)
*Web Apps, Function Apps, Logic Apps, Messaging Services*

[Previous content unchanged - 14 scripts including web apps, functions, etc.]

### **📊 Monitoring-Operations** (21 scripts)
*Monitoring, Performance, Health Checks, Automation Management*

[Previous content unchanged - 21 scripts including monitoring, alerts, etc.]

---

## 📈 **Updated Script Statistics**

| Folder | V4.0 | New Added | **V5.0 Total** | Growth | **% of Collection** |
|--------|------|-----------|-----------------|--------|---------------------|
| **🖥️ Compute-Management** | 31 | **+0** | **31** | **0%** | **28%** |
| **📊 Monitoring-Operations** | 21 | **+0** | **21** | **0%** | **19%** |
| **🌐 Network-Security** | 19 | **+0** | **19** | **0%** | **17%** |
| **💾 Data-Storage** | 15 | **+0** | **15** | **0%** | **13%** |
| **🚀 App-Development** | 14 | **+0** | **14** | **0%** | **13%** |
| **👥 Identity-Governance** | 3 | **+9** | **12** | **300%** | **11%** |
| **TOTAL** | **103** | **+9** | **112** | **9%** | **100%** |

---

## 🌟 **9 New Identity & Governance Scripts Added**

### **🔐 Core Identity Management:**
1. **Azure Service Principal Creator** - Automates service principal creation for CI/CD
2. **Azure AD Group Creator** - Manages Azure AD groups with bulk member addition
3. **Azure Managed Identity Creator** - Creates managed identities for secure access
4. **Azure Custom Role Creator** - Creates custom RBAC roles with fine-grained permissions

### **🛡️ Advanced Security & Access Control:**
5. **Azure Role Assignment Manager** - Manages role assignments across resources
6. **Azure PIM Role Activator** - Just-in-time privileged access activation
7. **Azure Conditional Access Policy Creator** - Zero Trust security policies
8. **Azure Access Review Creator** - Periodic access certification and compliance

### **📋 Governance & Compliance:**
9. **Azure Subscription Security Auditor** - Comprehensive security posture assessment

---

## 💡 **Enterprise Identity & Security Scenarios**

### **Complete Identity & Access Management Setup:**
```powershell
# 1. Create Service Principals for Automation
.\Identity-Governance\Azure-ServicePrincipal-Creator.ps1 -DisplayName "DevOps-Automation" -Role "Contributor"
.\Identity-Governance\Azure-ServicePrincipal-Creator.ps1 -DisplayName "Backup-Service" -Role "Backup Contributor"

# 2. Create Managed Identities for Applications
.\Identity-Governance\Azure-ManagedIdentity-Creator.ps1 -ResourceGroupName "App-RG" -IdentityName "WebApp-Identity" -Location "East US"

# 3. Create Custom Roles for Fine-Grained Access
.\Identity-Governance\Azure-Custom-Role-Creator.ps1 -RoleName "VM Operator" -Description "Start/Stop VMs only" -Actions @("Microsoft.Compute/virtualMachines/start/action", "Microsoft.Compute/virtualMachines/powerOff/action")

# 4. Create Azure AD Groups for Access Management
.\Identity-Governance\Azure-AD-Group-Creator.ps1 -GroupName "Database Administrators" -Description "DB Admin Access" -MemberEmails @("admin1@company.com", "admin2@company.com")

# 5. Assign Roles to Groups
.\Identity-Governance\Azure-Role-Assignment-Manager.ps1 -PrincipalId "group-object-id" -RoleDefinitionName "SQL DB Contributor" -Scope "/subscriptions/sub-id"
```

### **Enterprise Security & Compliance:**
```powershell
# 1. Security Audit
.\Identity-Governance\Azure-Subscription-Security-Auditor.ps1 -SubscriptionId "12345678-1234-1234-1234-123456789012"

# 2. Conditional Access for Zero Trust
.\Identity-Governance\Azure-ConditionalAccess-Policy-Creator.ps1 -PolicyName "Require MFA for Admins" -Description "MFA required for admin roles"

# 3. Access Reviews for Compliance
.\Identity-Governance\Azure-Access-Review-Creator.ps1 -ReviewName "Quarterly Admin Review" -GroupId "admin-group-id" -DurationInDays 14

# 4. PIM for Just-in-Time Access
.\Identity-Governance\Azure-PIM-Role-Activator.ps1 -RoleName "Global Administrator" -ResourceScope "/subscriptions/sub-id" -DurationHours 2 -Justification "Emergency system maintenance"

# 5. Policy-Based Governance
.\Identity-Governance\Azure-Policy-Assignment-Creator.ps1 -PolicyDefinitionId "/providers/Microsoft.Authorization/policyDefinitions/policy-id" -AssignmentName "Require Tags" -Scope "/subscriptions/sub-id"
```

### **DevOps Security Integration:**
```powershell
# 1. Create Service Principal for CI/CD Pipeline
.\Identity-Governance\Azure-ServicePrincipal-Creator.ps1 -DisplayName "GitHub-Actions-SP" -Role "Contributor" -Scope "/subscriptions/sub-id/resourceGroups/Production-RG"

# 2. Create Managed Identity for Application
.\Identity-Governance\Azure-ManagedIdentity-Creator.ps1 -ResourceGroupName "Production-RG" -IdentityName "ProductionApp-Identity" -Location "East US" -Role "Key Vault Secrets User" -Scope "/subscriptions/sub-id/resourceGroups/Production-RG/providers/Microsoft.KeyVault/vaults/ProductionKV"

# 3. Custom Role for Limited Access
.\Identity-Governance\Azure-Custom-Role-Creator.ps1 -RoleName "App Deployer" -Description "Deploy applications only" -Actions @("Microsoft.Web/sites/*", "Microsoft.Web/serverfarms/read")

# 4. Security Validation
.\Identity-Governance\Azure-Subscription-Security-Auditor.ps1 -SubscriptionId "prod-subscription-id" -OutputPath "Production-Security-Audit.html"
```

---

## 🏆 **Enterprise Identity & Governance Features**

### **🔐 Complete Identity Management:**
- Service principal automation for CI/CD pipelines
- Managed identity creation for secure application access
- Azure AD group management with bulk operations
- Custom RBAC role creation for fine-grained permissions

### **🛡️ Advanced Security Controls:**
- Role assignment management across resources
- Privileged Identity Management (PIM) integration
- Conditional Access policy automation
- Comprehensive security auditing and reporting

### **📋 Governance & Compliance:**
- Policy-based governance automation
- Access review creation for compliance
- Security posture assessment and recommendations
- Audit trails and compliance reporting

### **🚀 Enterprise Benefits:**
- **Zero Trust Security** - Conditional access and identity verification
- **Least Privilege Access** - Custom roles and just-in-time access
- **Automated Compliance** - Regular access reviews and policy enforcement
- **Security Monitoring** - Continuous auditing and alerting
- **DevOps Integration** - Service principals and managed identities for automation

---

## 📊 **Identity & Governance Coverage Matrix**

| **Capability** | **Scripts** | **Enterprise Value** |
|----------------|-------------|---------------------|
| **Identity Creation** | 4 scripts | Service principals, groups, managed identities |
| **Access Management** | 4 scripts | Role assignments, PIM, conditional access |
| **Governance** | 3 scripts | Policies, auditing, access reviews |
| **Compliance** | 2 scripts | Security audits, access certification |
| **User Management** | 1 script | Bulk offboarding automation |

---

## 📞 **Support & Contact**

**Wesley Ellis**  
📧 Email: wes@wesellis.com  
<<<<<<< HEAD:README.md
🌐 Website: wesellis.com
=======
🌐 Website: wesellis.com  
>>>>>>> 37dd711e9bf20eb9d0b0ad38da7ab0f3cda25fe6:scripts/README.md

---

## 📅 **Version History**

- **v5.0** (May 23, 2025) - Enhanced Identity & Governance with 9 new scripts (112 total)
- **v4.0** (May 23, 2025) - Added 25 advanced enterprise scripts (103 total)
- **v3.0** (May 23, 2025) - Added 25 essential scripts, organized into folders (78 total)
- **v2.0** (May 23, 2025) - Complete professional rewrite with enhanced functionality (53 total)
- **v1.0** (December 2024) - Initial script collection

---

*This is the ultimate Azure automation toolkit - 112 professional scripts with complete Identity & Governance coverage. Ready for enterprise security, compliance, and Zero Trust architecture deployment.*
