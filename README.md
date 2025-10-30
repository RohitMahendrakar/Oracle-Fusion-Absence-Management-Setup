Here’s your README rewritten in a **clean, professional, and visually appealing GitHub format** — same content, but with **consistent Markdown**, better spacing, link formatting, and emoji alignment for a modern look.

You can copy this directly into your `README.md` file.
All the references (`[1]`, `[2]`, etc.) are kept intact for easy maintenance.

---

````{"id":"59290","variant":"standard","title":"Oracle Fusion — Absence Management Module (Final README)"}
# 🧭 Oracle Fusion — Absence Management Module

> A concise, GitHub-ready README describing the **Absence Management configuration and processes** implemented in **Oracle Fusion HCM**.  
> Includes configuration tasks, transactional flows, and a clear explanation of absence plan/type concepts (accrual, entitlement, qualification, etc.).

---

## 📘 Overview

This repository documents the **Absence Management** setup and processes in **Oracle Fusion HCM**.  
The module helps organizations manage **employee leaves, accruals, entitlements, carryover rules, and automation** — ensuring accurate leave balances and compliance across HR, managers, and employees.  
([Oracle Docs][1])

---

## ⚙️ Key Configuration Tasks

*(These tasks were performed in the Absences work area.)*

- **Manage Derived Factors** — Create calculated factors (e.g., *length of service*, *age*) used to compute entitlements and eligibility.  
- **Manage Eligibility Profile** — Group employees by criteria (job, location, grade, org) to control who can enroll in plans.  
- **Manage Time Periods** — Define accrual and reporting periods (monthly, yearly, or custom).  
- **Manage Global Absence Lookups** — Standardize codes/values used across absence configurations.  
- **Manage Global Absence Descriptive Flexfields (DFFs)** — Add custom fields for organization-specific data capture.  
- **Manage Absence Reasons** — List standard reasons (e.g., *Sick*, *Vacation*, *Parental*, *Bereavement*).  
- **Manage Absence Plans** — Create plans that govern accrual, entitlement, carryover, limits, and rules.  
- **Manage Absence Certifications** — Configure medical or other certification requirements for certain absences.  
- **Manage Absence Types** — Map business leave categories (paid, unpaid, accrual-based, entitlement-based) to plans.  
- **Manage Work Shifts / Work Day Patterns / Work Schedules** — Set shift times and working patterns to calculate absence duration correctly.  
- **Manage Calendar Events** — Configure organization holidays and events that influence leave calculations.

> These tasks follow **Oracle Fusion best practices** for building end-to-end absence management flows.  
> ([Oracle Docs][1])

---

## 🧾 Absence Plan & Type Definitions

Oracle Fusion supports multiple **plan types** and **absence behaviours**.  
Below are concise definitions useful for configuration documentation and understanding plan functionality.

### 🗂️ Plan Types (created via *Absence Plans*)

- **Accrual Plan** — Employees earn leave over time (hours/days per pay period). Commonly used for PTO or vacation where balances grow gradually.  
  *Example:* accrue 1.67 days per month. ([Oracle Docs][2])

- **Qualification Plan** — Entitlement is determined by meeting qualification rules (e.g., *minimum service period*) before entitlement is granted. ([Oracle Docs][1])

- **No Entitlement Plan** — The absence is tracked but not entitled (used for unpaid or statutory leaves). ([Oracle Docs][2])

- **Agreement Plan** — Behaviour is based on collective or company agreements (e.g., *union agreements*). ([Oracle Docs][2])

- **Compensatory Plan** — Time off earned in exchange for extra hours worked (*comp time*). ([Oracle Docs][2])

- **Donation Plan** — Employees donate leave balance to another employee (where supported). ([Oracle Docs][3])

---

### 🧠 Common Absence Behaviours & Concepts

- **Accrual** — Mechanism to accumulate leave over time (periodic increments). Accruals can be monthly, weekly, banded, or grant-based. ([Oracle Docs][1])  
- **Entitlement** — The total leave an employee is eligible to use (fixed grant, qualification-based, or derived from accruals).  
  *Example:* maternity entitlement, statutory sick entitlement. ([Oracle][4])  
- **Carryover / Carry Forward** — Allows unused accruals to move into the next period up to defined limits or expiry rules. ([Oracle Docs][1])  
- **Certification** — Documentation requirement (e.g., medical certificate) enforced by the plan before entitlement approval. ([Oracle Docs][1])  
- **Adjustments / Disbursements** — Manual or automated operations used to correct balances or disburse cash when supported. ([Oracle Docs][1])

> Oracle supports **accrual-based**, **entitlement-based**, and **rule-based** absence types (e.g., *Bereavement*), offering flexibility to model both **business** and **statutory** requirements.  
> ([Oracle][4])

---

## 👥 Transaction Flows — Roles & Responsibilities

### 👩‍💼 HR / Absence Administrator
- Enroll employees into absence plans (based on eligibility).  
- Configure accrual rules, carryover, and plan limits.  
- Run **accrual** and **balance calculation** processes and reconcile results.  
- Update or correct plan enrollments and perform balance adjustments.  
- Configure certifications, lookups, and descriptive flexfields (DFFs).

### 🧑‍💻 Employee (Self-Service)
- Submit leave requests (choose type, dates, and reason).  
- View balances and leave history (entitlements, accruals, consumption).

### 👨‍🏫 Manager / Administrator (Self-Service)
- Approve or reject leave requests for direct reports.  
- Apply leave on behalf of employees (where permitted).  
- Monitor scheduled processes (accrual runs, evaluations, exceptions).  
- Automate recurring jobs for accrual runs, plan updates, and reporting.  
([Oracle][5])

---

## 🗂️ Repository Structure

```
Oracle-Fusion-Absence-Management/
├── README.md                <-- (this file)
├── screenshots/             <-- all screenshots in one folder
├── configs/                 <-- configuration exports or reference files
├── process_docs/            <-- HR & absence process notes
└── examples/                <-- sample plan definitions or templates
```

All screenshots are stored inside the `/screenshots` folder for simplicity.

---

## 📚 Sources & References

- Oracle Cloud HCM — *Types of Absence Plans* and Absence Management implementation docs. ([Oracle Docs][2])  
- Oracle Absence Management Datasheet — explains accrual-based and entitlement-based plan support. ([Oracle][4])  
- Leave & Accrual HR best practices — definitions of accrual, entitlement, and carryover. ([Shiftbase][6])

---

[1]: https://docs.oracle.com/en/cloud/saas/human-resources/24d/fahcm/index.html  
[2]: https://docs.oracle.com/en/cloud/saas/human-resources/24d/fahcm/define-absence-plans.html  
[3]: https://docs.oracle.com/en/cloud/saas/human-resources/24d/fahcm/absence-plan-donation.html  
[4]: https://www.oracle.com/applications/human-capital-management/absence-management/  
[5]: https://docs.oracle.com/en/cloud/saas/human-resources/24d/fahcm/manage-absences.html  
[6]: https://www.shiftbase.com/blog/accrual-vs-entitlement-leave

---

⭐ **Author:** Rohit Anand  
📍 *Bangalore, India*  
💼 *Oracle HCM Functional Enthusiast | Cloud Learner*  


---
````





