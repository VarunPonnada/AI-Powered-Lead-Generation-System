# Roles

## Overview

A **Role** in Salesforce defines a user's position within the organization's hierarchy and controls **record-level data visibility**. Roles determine which records users can view based on the role hierarchy. Users higher in the hierarchy can typically access records owned by users below them.

Roles do **not** grant object or field permissions; those are managed through **Profiles** and **Permission Sets**.

---

## Navigation Steps

### 1. Access Salesforce Setup

- Log in to Salesforce.
- Click the **⚙️ Gear** icon in the top-right corner.
- Select **Setup**.

---

### 2. Navigate to Roles

- In the **Quick Find** search box, type **Roles**.
- Under **Users**, click **Roles**.
- The **Role Hierarchy** page opens, displaying the existing organization hierarchy.

---

### 3. Create a New Role

1. On the Role Hierarchy page, click **Add Role** under the desired parent role.
2. Enter the following details:
   - **Role Label**
   - **Role Name**
   - **This Role Reports To** (Parent Role)
   - **Role Name as Displayed on Reports**
3. Click **Save**.

---

### 4. Edit an Existing Role

1. On the Role Hierarchy page, locate the role.
2. Click **Edit**.
3. Modify the role information as required.
4. Click **Save**.

---

### 5. Assign Users to a Role

1. Go to **Setup → Users → Users**.
2. Open or edit the desired user.
3. Select the appropriate **Role**.
4. Click **Save**.

---

# Activity 1: Create Lead Manager Role

### Step 1

Go to:

**Setup → Roles**

---

### Step 2

On the Role Hierarchy page:

- Click **Add Role** under **CEO** (or any suitable upper-level role if required).

---

### Step 3

Enter the following details:

| Field | Value |
|--------|-------|
| Role Label | Lead Manager |
| Role Name | Lead_Manager |
| This Role Reports To | CEO |
| Role Name as Displayed on Reports | Lead Manager |

---

### Step 4

Click **Save**.

---

# Activity 2: Create Sales Agent Role

### Step 1

Return to the **Role Hierarchy**.

---

### Step 2

Click **Add Role** directly under **Lead Manager**.

---

### Step 3

Enter the following details:

| Field | Value |
|--------|-------|
| Role Label | Sales Agent |
| Role Name | SalesAgent *(or Sales_Agent if available)* |
| This Role Reports To | Lead Manager |
| Role Name as Displayed on Reports | Sales Agent |

---

### Step 4

Click **Save**.

---

## Final Role Hierarchy

```text
Ideal Institute Of Technology
├── CEO
├── CFO
├── COO
├── Lead Manager
│   └── Sales Agent
├── SVP, Customer Service & Support
├── SVP, Human Resources
└── SVP, Sales & Marketing
```

---

## Result

Successfully created:

- Lead Manager Role
- Sales Agent Role

Configured the role hierarchy so that:

- **Sales Agent** reports to **Lead Manager**.
- **Lead Manager** reports to **CEO**.

This hierarchy enables proper record-level visibility according to Salesforce's role-based access model.
