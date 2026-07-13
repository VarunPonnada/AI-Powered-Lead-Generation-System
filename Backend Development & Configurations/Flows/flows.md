# Flows
## AI-Powered Lead Generation System

## 1. Overview

Salesforce Flows are declarative automation tools that enable organizations to automate business processes without writing code. Flows can create, update, delete, and retrieve records, send emails, perform calculations, and execute business logic automatically.

In this project, a **Record-Triggered Flow** is implemented to automatically send an email to a Lead whenever a Lead record is created or updated.

---

## 2. Objective

The objective of this flow is to automate lead communication by sending an email containing the AI-generated lead summary immediately after a Lead record is created or updated.

---

## 3. Navigate to Flow Builder

1. Log in to Salesforce Developer Edition.
2. Click the **⚙️ Gear** icon.
3. Select **Setup**.
4. In the **Quick Find** search box, search for **Flows**.
5. Select **Flows**.
6. Click **New Flow**.

---

## 4. Select Flow Type

Configure the flow as follows:

| Property | Value |
|----------|-------|
| Category | Triggered |
| Flow Type | Record-Triggered Flow |

Click **Create**.

---

## 5. Configure the Start Element

Configure the Start element using the following settings.

| Property | Value |
|----------|-------|
| Object | Lead |
| Trigger | A record is created or updated |
| Condition Requirements | None |
| Optimize the Flow For | Actions and Related Records |
| When to Run | Run Immediately |

Click **Done**.

---

## 6. Add the Send Email Action

1. Click the **+** icon below the **Start** element.
2. Select **Action**.
3. Search for **Send Email**.
4. Select the **Send Email** action.

---

## 7. Configure the Email Action

Configure the action using the following values.

| Property | Value |
|----------|-------|
| Label | Send Lead Email |
| Subject | Lead Information |
| Recipient Addresses | Triggering Lead → Email |
| Sender Type | Current User |
| Related Record ID | Triggering Lead → Lead ID |

### Email Body

```
Hello {!$Record.FirstName} {!$Record.LastName},

Thank you for your interest.

AI Summary:
{!$Record.AI_Summary__c}

Regards,
Sales Team
```

After configuring the action, click **Done**.

---

## 8. Save the Flow

Save the flow using the following details.

| Property | Value |
|----------|-------|
| Flow Label | Send Lead Email Flow |
| API Name | Send_Lead_Email_Flow |

Click **Save**.

---

## 9. Activate the Flow

After saving:

1. Click **Activate**.
2. Verify that the flow status changes to **Active**.

---

## 10. Test the Flow

To verify the automation:

1. Navigate to the **Sales** application.
2. Open the **Leads** tab.
3. Create a new Lead record.
4. Enter all required details, including:
   - First Name
   - Last Name
   - Company
   - Email
   - Lead Score
   - Lead Category
   - Product Interest
   - AI Summary
5. Save the record.

The flow automatically sends an email to the Lead using the configured email address.

> **Note:** If the **Reject_Personal_Email** validation rule is active, temporarily deactivate it while testing with a personal email address. Reactivate the validation rule after testing is complete.

---

## 11. Verification

The flow was successfully tested by creating a Lead record. Upon saving the record, Salesforce automatically executed the Record-Triggered Flow and sent an email containing the AI-generated lead summary to the specified recipient.

---

## Outcome

The Record-Triggered Flow was successfully implemented and activated. The automation reduces manual effort by automatically notifying leads with AI-generated information whenever a Lead record is created or updated. This demonstrates Salesforce Flow Builder's capability to automate business processes without writing Apex code.
