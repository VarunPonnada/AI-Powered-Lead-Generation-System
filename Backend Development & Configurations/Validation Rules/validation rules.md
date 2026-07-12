# Validation Rules
## AI-Powered Lead Generation System

## 1. Overview

Validation Rules in Salesforce ensure that records meet specific business requirements before they are saved. They help maintain data accuracy by preventing users from entering invalid or unwanted information.

In this project, a validation rule is created on the **Lead** object to prevent users from using personal email addresses (such as Gmail, Yahoo, Hotmail, and Outlook) when creating Lead records.

---

## 2. Navigate to Validation Rules

1. Log in to your Salesforce Developer Org.
2. Click the **⚙️ Gear Icon** in the upper-right corner.
3. Select **Setup**.
4. Click **Object Manager**.
5. Search for and select the **Lead** object.
6. In the left sidebar, click **Validation Rules**.
7. Click **New**.

---

## 3. Configure the Validation Rule

Fill in the following details:

| Field | Value |
|-------|-------|
| Rule Name | Reject_Personal_Email |
| Active | Checked |
| Description | Prevents users from entering personal email addresses for Lead records. |

---

## 4. Enter the Error Condition Formula

Copy and paste the following formula into the **Error Condition Formula** section:

```text
OR(
    CONTAINS(Email, "@gmail."),
    CONTAINS(Email, "@yahoo."),
    CONTAINS(Email, "@hotmail."),
    CONTAINS(Email, "@outlook.")
)
```

Click **Check Syntax** to verify that the formula contains no errors.

---

## 5. Configure the Error Message

Fill in the following details:

| Field | Value |
|-------|-------|
| Error Message | Personal email domains like Gmail, Yahoo, Hotmail, and Outlook are not allowed. |
| Error Location | Field |
| Field | Email |

---

## 6. Save the Validation Rule

1. Click **Save**.
2. The validation rule is now active and will be applied whenever a Lead record is created or updated.

---

## 7. Verify the Validation Rule

To verify the validation rule:

1. Open the **Sales** application.
2. Navigate to **Leads**.
3. Click **New**.
4. Enter the Lead details.
5. In the **Email** field, enter a personal email address (for example, `test@gmail.com`).
6. Click **Save**.

Salesforce should display the following error message:

> Personal email domains like Gmail, Yahoo, Hotmail, and Outlook are not allowed.

This confirms that the validation rule is working correctly.

---

## Expected Outcome

- Personal email domains such as Gmail, Yahoo, Hotmail, and Outlook are rejected.
- Users must provide valid business email addresses.
- Lead data quality and consistency are improved throughout the CRM system.
