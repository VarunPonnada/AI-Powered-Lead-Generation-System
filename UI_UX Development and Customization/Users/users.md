# Users Configuration

## Overview

A **User** in Salesforce represents an individual who can log in to the Salesforce organization. Every user is assigned a **Profile**, which determines their permissions and access level. Users can also be assigned **Roles**, **Permission Sets**, and **Licenses** to control data visibility and functionality.

---

# Activity 1: Create Lead Manager User

## Objective

Create a new user with the **Lead Manager Profile** to manage lead-related activities.

---

### Step 1: Open Users

1. Log in to Salesforce.
2. Click the **⚙️ Gear** icon.
3. Select **Setup**.
4. In the **Quick Find** box, search for **Users**.
5. Under **Users**, click **Users**.
6. Click **New User**.

---

### Step 2: Enter User Details

Fill in the required information.

| Field | Value |
|--------|-------|
| First Name | Lead |
| Last Name | Manager |
| Alias | lead |
| Email | Your personal email |
| Username | salesagent@test.com *(must be globally unique)* |
| Nickname | leadmanager |
| Role | Lead Manager |
| User License | Salesforce |
| Profile | Lead Manager Profile |

> **Note:** The username must be globally unique. If `salesagent@test.com` is already in use, append a unique suffix (for example, `salesagent2026@test.com`).

---

### Step 3: Save the User

Click **Save**.

---

### Step 4: Verify Login

1. Log out of Salesforce.
2. Go to the Salesforce login page.
3. Click **Forgot Password**.
4. Enter the new username.
5. Check your email for the password reset link.
6. Create a new password.
7. Log in using the newly created credentials.

---

# Activity 2: Create Sales Agent User

## Objective

Create a Sales Agent user with limited access for lead management.

---

### Step 1: Open Users

Navigate to:

**Setup → Users → Users**

Click **New User**.

---

### Step 2: Enter User Details

| Field | Value |
|--------|-------|
| First Name | Sales |
| Last Name | Agent |
| Alias | sales |
| Email | Your personal email |
| Username | salesagent@test.com *(must be globally unique)* |
| Nickname | salesagent |
| Role | Sales Agent |
| User License | Salesforce |
| Profile | Sales Agent Profile |

> **Note:** If the username already exists, create a unique username such as `salesagent2026@test.com`.

---

### Step 3: Save the User

Click **Save**.

---

# Edit an Existing User

1. Go to **Setup → Users → Users**.
2. Locate the required user.
3. Click **Edit**.
4. Update the necessary information such as:
   - Profile
   - Role
   - Email Address
   - Time Zone
   - Active Status
5. Click **Save**.

---

# Activate, Deactivate, or Freeze a User

## Deactivate a User

1. Open the user record.
2. Click **Edit**.
3. Uncheck **Active**.
4. Click **Save**.

---

## Freeze a User

1. Open the user record.
2. Click **Freeze**.

Freezing temporarily prevents the user from logging in without deactivating the account.

---

# Reset a User Password

1. Navigate to **Setup → Users → Users**.
2. Locate the required user.
3. Click **Reset Password**.
4. Salesforce sends a password reset email to the registered email address.

---

# Assign Permission Sets (Optional)

1. Open the user record.
2. Scroll to **Permission Set Assignments**.
3. Click **Edit Assignments**.
4. Select the required permission set.
5. Click **Add**.
6. Click **Save**.

---

# User Information Summary

| Field | Description |
|--------|-------------|
| First Name | User's first name |
| Last Name | User's last name |
| Alias | Short identifier displayed in Salesforce |
| Email | Email address used for notifications |
| Username | Globally unique login ID |
| Nickname | Chatter display name |
| Role | Determines record visibility through the role hierarchy |
| User License | Defines the Salesforce features available to the user |
| Profile | Determines object permissions, field permissions, and system access |

---

# Result

Successfully created and configured:

- Lead Manager User
- Sales Agent User

Each user was assigned the appropriate **Profile**, **Role**, and **User License**, allowing secure access based on their responsibilities within the AI-Powered Lead Generation System.
