# Profiles Configuration

## Overview

A **Profile** in Salesforce is a collection of settings and permissions that defines what a user can access and perform within the Salesforce platform. Profiles determine the level of access to objects, fields, applications, tabs, Apex classes, Visualforce pages, page layouts, record types, and various administrative features.

Profiles are generally assigned based on a user's job role. Examples include System Administrator, Sales Representative, Lead Manager, and Sales Agent.

---

# Activity 1: Create Lead Manager Profile

## Objective

Create a custom profile that provides complete access to Lead management activities.

### Step 1: Open Profiles

1. Log in to Salesforce.
2. Click **⚙️ Setup**.
3. In **Quick Find**, search for **Profiles**.
4. Select **Profiles**.

---

### Step 2: Clone an Existing Profile

1. Locate an existing profile (for example, **Standard User** or another suitable base profile such as **Contract Manager** if Standard User is unavailable).
2. Click **Clone**.

---

### Step 3: Enter Profile Details

Enter:

| Field | Value |
|--------|-------|
| Profile Name | Lead Manager Profile |

Click **Save**.

---

### Step 4: Configure Object Permissions

Edit the newly created profile.

Grant the following permissions.

#### Lead

- Read
- Create
- Edit
- Delete

(Optional)

- Modify All

#### Contact

- Read
- Create
- Edit
- Delete

#### Task

- Read
- Create
- Edit
- Delete

#### Event

- Read
- Create
- Edit
- Delete

---

### Step 5: Configure Field-Level Security

Navigate to:

**Setup → Object Manager → Lead → Fields & Relationships**

Open the required field.

Click **Set Field-Level Security**.

Grant visibility to the required profiles.

Click **Save**.

---

### Step 6: Configure App & System Permissions

Within the profile, enable permissions as required.

For this project:

- API Enabled
- Other permissions according to project requirements

---

### Step 7: Save

Click **Save** to apply all profile changes.

---

# Activity 2: Create Sales Agent Profile

## Objective

Create a restricted profile for sales representatives responsible for managing leads.

---

### Step 1: Open Profiles

Go to:

**Setup → Profiles**

---

### Step 2: Clone an Existing Profile

Clone an existing profile.

---

### Step 3: Enter Profile Details

| Field | Value |
|--------|-------|
| Profile Name | Sales Agent Profile |

Click **Save**.

---

### Step 4: Configure Object Permissions

#### Lead

- Read
- Create
- Edit

Do **not** grant:

- Delete

#### Contact

- Read

#### Task

- Read
- Create
- Edit

#### Event

- Read
- Create
- Edit

---

### Step 5: Configure User Permissions

Enable:

- View Reports

Grant any additional permissions required for sales users.

---

### Step 6: Save

Click **Save**.

---

# Features of Salesforce Profiles

A Salesforce Profile controls access to:

- Objects
- Fields
- Applications
- Tabs
- Apex Classes
- Visualforce Pages
- Record Types
- Page Layouts
- Login Hours
- Login IP Ranges
- Administrative Permissions
- General User Permissions

---

# Result

Successfully created and configured:

- Lead Manager Profile
- Sales Agent Profile

The Lead Manager profile provides full Lead management capabilities, while the Sales Agent profile offers controlled access suitable for day-to-day sales operations following the principle of least privilege.
