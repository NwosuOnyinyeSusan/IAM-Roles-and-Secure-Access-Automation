# IAM-Roles-and-Secure-Access-Automation
Capstone Project: IAM Roles and Secure Access Automation using AWS CLI

📘 Project Title

IAM Roles and Secure Access Automation Project


---

📄 Project Overview

This project demonstrates how to implement Identity and Access Management (IAM) controls using AWS CLI for automation.
It replaces a similar Azure-based objective with an AWS approach — focusing on automating the creation of IAM roles, user groups, and permission boundaries while ensuring secure and controlled access to cloud resources.

The project validates role-based access control (RBAC) by testing read-only permissions for two groups — DBAdmins and WebAdmins — using automated configurations and verification through CLI profiles.


---

🎯 Objectives

Automate IAM group and policy creation using AWS CLI.

Enforce least privilege access across DB and Web environments.

Verify access permissions through test users and CLI profiles.

Demonstrate secure, scalable cloud access management principles.



---

🧩 Tools and Technologies

Platform: Amazon Web Services (AWS)

CLI Utility: AWS CLI v2

Operating System: Kali Linux

Version Control: Git & GitHub

Languages/Syntax: JSON, Bash

Documentation Tools: LibreOffice Writer / PowerPoint



---

🏗️ Project Folder Structure

IAM-Automation-Project/
│
├── policies/
│   ├── DBAdminsReadOnlyPolicy.json
│   └── WebAdminsReadOnlyPolicy.json
│
├── docs/
│   ├── IAM_Project_Report.pdf
│   └── IAM_Roles_Project_Slides.pptx
│
├── screenshots/
│   ├── vpc_creation.png
│   ├── subnets_creation.png
│   ├── iam_groups.png
│   ├── policy_attachment.png
│   └── permission_test_results.png
│
├── scripts/
│   └── (optional CLI automation scripts if added)
│
└── README.md


---

⚙️ Key Implementation Steps

1. Configured AWS CLI with verified credentials.


2. Created a VPC and two subnets (WebSubnet, DBSubnet) under unique CIDR ranges.


3. Created IAM groups:

DBAdmins

WebAdmins



4. Defined JSON policies for each group (DBAdminsReadOnlyPolicy, WebAdminsReadOnlyPolicy).


5. Created and attached IAM policies to the respective groups.


6. Added test users:

TestDBUser → DBAdmins

TestWebUser → WebAdmins



7. Generated and configured access keys for both users via AWS CLI.


8. Tested permissions — verified read-only success and denied delete operations.




---

💡 Challenges and Solutions

Challenge Description Solution

AWS CLI syntax errors Quotation marks and line continuation caused command failure. Used single-line commands with correct quotes and verified syntax.
Subnet conflicts Overlapping CIDR blocks prevented subnet creation. Adjusted subnet ranges (10.0.1.0/24 & 10.0.2.0/24).
Wrong policy attachment WebAdmins had wrong JSON file attached initially. Detached incorrect policy and reattached correct ARN.
Access key misconfiguration Duplicate or wrong key created. Deleted bad key, reconfigured profiles with correct credentials.



---

🧾 Results

✅ IAM groups and policies successfully automated.
✅ Verified least-privilege enforcement.
✅ VPC and subnets properly segmented.
✅ Access validation confirmed — delete operations denied for both test users.
✅ Documentation and slides prepared for presentation.


---

🧠 Key Takeaways

Proper IAM structure prevents unauthorized actions.

AWS CLI enables repeatable, auditable automation.

Documentation and tagging simplify environment management.

Separate profiles simulate realistic user access testing.



---

🧱 References

AWS Identity and Access Management Documentation

AWS CLI Command Reference

AWS Security Best Practices Whitepaper

TechCrush Capstone Project Guide



---

👤 Author

Onyinye Nwosu
Capstone Project — TechCrush
AWS Identity & Access Management (IAM) Automation
