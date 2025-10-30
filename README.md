# 🧭 Oracle Fusion — Absence Management Module

> A professional and visually rich README for the **Absence Management configuration and processes** implemented in **Oracle Fusion HCM**.
> Includes setup components, transactional workflows, and a clear breakdown of absence plan types like **Accrual**, **Entitlement**, and **Qualification**.

---

## 📘 Overview

This repository documents the **Absence Management** module setup in **Oracle Fusion HCM**.
It provides a structured explanation of configurations, plan types, and process flows across **HR**, **Managers**, and **Employees** — enabling streamlined leave management, automation, and compliance.
([Oracle Docs][1])

---

## ⚙️ Configuration Components

Below are the core configuration tasks performed in the **Absence Management** work area:

* ⚖️ **Manage Derived Factors** — Create calculated metrics like *Length of Service* or *Age* to determine eligibility and entitlement.
* 🧩 **Manage Eligibility Profile** — Define which employees qualify for a plan based on roles, grades, or locations.
* 📅 **Manage Time Periods** — Set up accrual and reporting periods (monthly, yearly, or fiscal).
* 🌐 **Manage Global Absence Lookups** — Maintain standardized lookup codes used across the application.
* 🧾 **Manage Global Absence DFFs (Descriptive Flexfields)** — Add organization-specific data capture fields.
* 🧍 **Manage Absence Reasons** — Define business-specific leave reasons (*Sick*, *Vacation*, *Maternity*, etc.).
* 🧮 **Manage Absence Plans** — Configure accrual rules, carryover, limits, and disbursement options.
* 📑 **Manage Absence Certifications** — Require supporting documentation for absences like *Medical Leave*.
* 🗂️ **Manage Absence Types** — Classify absences by behavior (*Accrual-based*, *Entitlement-based*, *Qualification-based*).
* 🕒 **Manage Work Shifts, Day Patterns & Schedules** — Define working time structures for accurate duration calculation.
* 📆 **Manage Calendar Events** — Record organizational holidays that affect absence calculations.

---

## 🧾 Absence Plan Types

Oracle Fusion supports multiple **absence plan categories** — each serving different business or statutory needs.

### 🗂️ **1. Accrual Plan**

Employees earn leave progressively based on time worked (e.g., per pay period or month).
*Example:* 1.67 days accrued monthly.
Used for **Paid Time Off (PTO)**, **Annual Leave**, or **Vacation**.

### 🎯 **2. Entitlement Plan**

Fixed leave granted upfront at the start of a period (e.g., 12 casual leave days per year).
Ideal for **Statutory Leave** or **One-time grants**.

### 🧮 **3. Qualification Plan**

Leave is granted only when an employee meets certain criteria (e.g., *minimum 2 years of service*).
Used for **Long Service Leave** or **Special Leave**.

### ⚙️ **4. Compensatory Plan**

Employees earn time-off for extra hours worked (Comp-Off).
Balances depend on approved overtime entries.

### 🤝 **5. Agreement Plan**

Rules derived from collective or union agreements defining specific leave rights.

### 💝 **6. Donation Plan**

Allows employees to donate leave balances to colleagues (where enabled).

---

## 🧠 Key Concepts

| Concept                            | Description                                                        |
| ---------------------------------- | ------------------------------------------------------------------ |
| 🕓 **Accrual**                     | Process of periodically adding leave to an employee’s balance.     |
| 🎟️ **Entitlement**                | The total amount of leave an employee is eligible to use.          |
| 🔁 **Carryover**                   | Transfer of unused leave to the next period within defined limits. |
| 🩺 **Certification**               | Supporting document required for specific absences.                |
| ⚖️ **Adjustments / Disbursements** | Manual corrections or payouts of accrued leave.                    |

> Oracle’s flexible model allows hybrid leave systems — combining **accrual-based**, **entitlement-based**, and **qualification-based** plans.
> ([Oracle][4])

---

## 👥 Role-Based Transaction Flows

### 👩‍💼 HR Administrator

* Enroll employees in absence plans.
* Run **Accrual Calculation** and **Balance Updates**.
* Adjust balances and update plan configurations.
* Review plan enrollments, disbursements, and exceptions.
* Monitor absence-related scheduled processes.

### 🧑‍💻 Employee (Self-Service)

* Apply for leaves and view current balances.
* Track approval status and leave history.
* Submit certifications if required.

### 👨‍🏫 Manager / Approver

* Approve or reject employee absence requests.
* Apply leave on behalf of subordinates (if authorized).
* Oversee absence analytics and ensure business continuity.

---

## 🧩 HR Transactions Overview

| Process                                          | Description                                               |
| ------------------------------------------------ | --------------------------------------------------------- |
| 🪪 **Absence Plan Enrollment**                   | Assigns employees to plans based on eligibility.          |
| 📊 **Calculate Accrual & Balances**              | Executes accrual process to update balances.              |
| 🧾 **Update Plan Enrollment**                    | Modifies or corrects existing enrollments.                |
| 💸 **Accrual Balance Disbursement**              | Converts leave to monetary disbursement if enabled.       |
| 🔧 **Adjusting Balances**                        | Manual corrections by HR admin.                           |
| 🧍 **Employee Self-Service Leave Application**   | Employee applies for leave through self-service portal.   |
| 🧑‍💼 **Manager Self-Service Leave Application** | Manager applies or approves leave for team members.       |
| 🕰️ **Schedule & Monitor Absence Processes**     | Monitor accrual jobs and leave-related automation.        |
| 🤖 **Automate the Schedule Process**             | Set recurring automation for accrual and balance updates. |

---


## 📚 References

* [Oracle HCM Cloud Absence Management Overview][4]
* [Defining Absence Plans — Oracle Docs][2]
* [Absence Plan Donation — Oracle Docs][3]
* [Oracle 24D HCM Documentation][1]
* [Shiftbase HR Blog — Accrual vs Entitlement][6]

---

[1]: https://docs.oracle.com/en/cloud/saas/human-resources/24d/fahcm/index.html
[2]: https://docs.oracle.com/en/cloud/saas/human-resources/24d/fahcm/define-absence-plans.html
[3]: https://docs.oracle.com/en/cloud/saas/human-resources/24d/fahcm/absence-plan-donation.html
[4]: https://www.oracle.com/applications/human-capital-management/absence-management/
[5]: https://docs.oracle.com/en/cloud/saas/human-resources/24d/fahcm/manage-absences.html
[6]: https://www.shiftbase.com/blog/accrual-vs-entitlement-leave

---


---

## 📝 Points to Remember

* Please **clone the project** instead of downloading individual files.  
* Cloning or downloading the **entire repository as a ZIP** will include all required folders and images.  
* After downloading, **unzip the project** — you’ll find all the **execution screenshots** inside the designated folder (e.g., `/screenshots/`).  
* The images may not open correctly if viewed through “Download Raw” on GitHub — this is expected.  
* Always open images **locally after extraction** to view the execution results clearly.




---

⭐ **Author:** Rohit Anand
📍 *Bangalore, India*
💼 *Oracle HCM Functional Enthusiast | Cloud Learner*

---
