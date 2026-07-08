# Objects Creation

## AI-Powered Lead Generation System

## 1. Overview

Custom Objects are used to store business-specific data that is not available in Salesforce's standard objects. For the **AI-Powered Lead Generation System**, custom objects help manage lead information, customer interactions, and project-specific data efficiently.

---

## 2. Access Salesforce Setup

1. Log in to your Salesforce Developer Organization.
2. Click the **⚙️ Gear** icon in the upper-right corner.
3. Select **Setup** from the dropdown menu.
4. The Salesforce Setup Home page will open.

---

## 3. Navigate to Object Manager

1. In the Setup page, click **Object Manager** from the top navigation bar.
2. A list of all Standard and Custom Objects will be displayed.

---

## 4. Create a New Custom Object

1. Click **Create** → **Custom Object** (or **New Custom Object**, depending on your Salesforce version).
2. The **Custom Object Definition** page will open.

---

## 5. Configure Custom Object Details

Fill in the required information.

### Basic Information

| Field | Description |
|--------|-------------|
| Label | Display name of the object (Example: Project) |
| Plural Label | Plural form of the object (Example: Projects) |
| Object Name | Automatically generated from the Label |
| Record Name | Choose **Text** or **Auto Number** |

If **Auto Number** is selected, specify the display format.

Example:

```
PROJ-{0000}
```

---

## 6. Enable Optional Features

Enable the required features according to project requirements.

- Allow Reports
- Allow Activities
- Track Field History
- Allow Search
- Allow Notes & Attachments
- Enable Streaming API
- Enable Enhanced Email

---

## 7. Configure Deployment Status

Select one of the following deployment options:

- **Deployed** – The object is available for users.
- **In Development** – The object remains hidden until development is completed.

---

## 8. Configure Object-Level Security

Configure the required permissions for the object.

Available options include:

- Allow Notes & Attachments
- Enable Sharing
- Allow Reports
- Allow Activities
- Allow Bulk API Access

These settings determine how users can interact with the custom object.

---

## 9. Save the Custom Object

Click **Save**.

The custom object is successfully created and its detail page will be displayed.

---

## Result

The custom object has been successfully created in Salesforce and is now ready to be used for developing the **AI-Powered Lead Generation System**.

---

## Conclusion

Creating custom objects allows Salesforce to store application-specific information that supports the business requirements of the AI-Powered Lead Generation System. These objects serve as the foundation for relationships, automation, validation rules, reports, and workflows developed in later stages of the project.
