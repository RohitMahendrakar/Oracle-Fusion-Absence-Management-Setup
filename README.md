---

# 🧭 Oracle Fusion — Absence Management Module

> A concise, GitHub-ready README describing the Absence Management configuration and processes implemented in Oracle Fusion HCM.
> Includes configuration tasks, transactional flows, and a clear explanation of absence plan/type concepts (accrual, entitlement, qualification, etc.).

---

## 📘 Overview

This repository documents the **Absence Management** setup and processes in **Oracle Fusion HCM**. The module helps organisations manage employee leaves, accruals, entitlements, carrying rules, and related automation — ensuring accurate leave balances and compliance across HR, managers, and employees. ([Oracle Docs][1])

---

## ⚙️ Key Configuration Tasks

(These tasks were performed in the Absences work area.)

* **Manage Derived Factors** — create calculated factors (e.g., length of service, age) used to compute entitlements and eligibility.
* **Manage Eligibility Profile** — group employees by criteria (job, location, grade, org) to control who can enroll in plans.
* **Manage Time Periods** — define accrual and reporting periods (monthly, yearly, custom).
* **Manage Global Absence Lookups** — standardize codes/values used across absence configs.
* **Manage Global Absence Descriptive Flexfields (DFFs)** — add custom fields for org-specific data capture.
* **Manage Absence Reasons** — list standard reasons (sick, vacation, parental, bereavement).
* **Manage Absence Plans** — create plans that govern accrual, entitlement, carryover, limits, and rules.
* **Manage Absence Certifications** — configure medical or other certification requirements for certain absences.
* **Manage Absence Types** — map business leave categories (paid, unpaid, accrual-based, entitlement-based) to plans.
* **Manage Work Shifts / Work Day Patterns / Work Schedules** — set shift times and working patterns to calculate absence duration correctly.
* **Manage Calendar Events** — configure organization holidays and events that influence leave calculations.

> These tasks follow Oracle Fusion best practices for building end-to-end absence management flows. ([Oracle Docs][1])

---

## 🧾 Absence Plan & Type Definitions (clear and practical)

Oracle Fusion supports multiple **plan types** and **absence behaviours**. Below are concise definitions to use in configuration docs and README notes.

### Plan types (create via *Absence Plans*):

* **Accrual Plan** — employees earn leave over time (hours/days per pay period). Used for PTO/vacation where balances grow by accrual rules. Example: accrue 1.67 days per month. ([Oracle Docs][2])
* **Qualification Plan** — entitlement is determined by meeting qualification rules (e.g., minimum service period) before entitlement is granted. ([Oracle Docs][1])
* **No Entitlement** — the absence is tracked but not entitled (used for tracking unpaid or unpaid stat leaves). ([Oracle Docs][2])
* **Agreement** — plan behavior based on specific agreements (e.g., company / union agreements). ([Oracle Docs][2])
* **Compensatory** — earned time off in exchange for extra hours worked (comp time). ([Oracle Docs][2])
* **Donation** — employees donate balance to another employee (where supported). ([Oracle Docs][3])

### Common absence behaviours / concepts:

* **Accrual** — the mechanism to accumulate leave over time (periodic increments). Accruals can be periodic (monthly/weekly), banded, or grant-based. ([Oracle Docs][1])
* **Entitlement** — the amount of leave an employee is eligible to use (could be a fixed grant, qualification-based, or derived from accruals). Examples: maternity entitlement, statutory sick entitlement. ([Oracle][4])
* **Carryover / Carry Forward** — rules that allow unused accruals to move into the next period up to defined limits or expiry rules. ([Oracle Docs][1])
* **Certification** — documentation requirement (e.g., medical certificate) enforced by the plan before further absence or entitlement is honored. ([Oracle Docs][1])
* **Adjustments / Disbursements** — manual or automated operations used to adjust balances or to disburse cash (if the plan supports monetary disbursement). ([Oracle Docs][1])

> Oracle explicitly supports accrual-based, entitlement-based, and simple rule-based absence types (e.g., bereavement), giving administrators flexibility to model business and statutory requirements. ([Oracle][4])

---

## 👥 Transaction Flows (who does what)

### HR / Absence Administrator

* Enroll employees into absence plans (based on eligibility).
* Configure accrual rules, carryover, and plan limits.
* Run accrual & balance calculation processes and reconcile results.
* Update or correct plan enrollments and manual adjustments.
* Configure certifications, lookups, and DFFs.

### Employee (Self-Service)

* Submit leave requests (select absence type, dates and reason).
* View balances and leave history (entitlements, accruals, consumed).

### Manager / Administrator (Self-Service)

* Approve or reject leave requests for direct reports.
* Apply leave on behalf of employees (where allowed).
* Monitor scheduled processes (accrual runs, evaluations) and exceptions.
* Setup automation for scheduled processes (accrual runs, enrollment updates). ([Oracle][5])

---


## 📚 Sources & References

* Oracle Cloud HCM — *Types of Absence Plans* and Absence Management implementation documents. ([Oracle Docs][2])
* Oracle Absence Management datasheet — describes accrual-based, entitlement-based, and rule-based absence support. ([Oracle][4])
* Leave/Accrual definitions and HR best-practices (accrual/entitlement/ carryover). ([shiftbase.com][6])

---


