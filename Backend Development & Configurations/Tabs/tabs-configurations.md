# Tabs Configuration
## AI-Powered Lead Generation System

## 1. Overview

Tabs in Salesforce are navigation elements that allow users to access specific objects, functionalities, or custom pages directly from the application interface. They act as entry points that provide quick access to records, list views, Lightning pages, Visualforce pages, or external content. Proper tab configuration improves navigation and enhances the overall user experience.

---

## 2. Access Salesforce Setup

1. Log in to your Salesforce Developer Org.
2. Click the **⚙️ Gear** icon in the upper-right corner.
3. Select **Setup** to open the Salesforce Setup page.

---

## 3. Navigate to the Tabs Section

1. In the **Quick Find** search box, type **Tabs**.
2. Under **User Interface**, click **Tabs**.
3. The Tabs page displays all available:
   - Standard Tabs
   - Custom Object Tabs
   - Visualforce Tabs
   - Lightning Page Tabs
   - Web Tabs

---

## 4. Create a New Custom Object Tab

1. Locate the **Custom Object Tabs** section.
2. Click **New**.
3. Select the custom object created for this project:

   **AI Lead Predictions**

4. Choose a suitable **Tab Style**.
5. (Optional) Add a description for internal reference.
6. Click **Next**.

---

## 5. Configure Tab Visibility

Configure the tab visibility for user profiles.

Available options include:

- **Default On** – The tab appears in the navigation bar by default.
- **Default Off** – Users can manually add the tab if needed.
- **Tab Hidden** – The tab is hidden for the selected profile.

For this project, **Default On** was selected for all profiles.

Click **Next**.

---

## 6. Add Tab to Applications

Select the Salesforce applications where the custom tab should be available.

For this project, the tab was added to the **Sales App**.

Click **Save** to complete the configuration.

---

## 7. Verification

After saving the configuration:

1. Open the **Sales** application.
2. Verify that the **AI Lead Predictions** tab appears in the navigation bar.
3. Open the tab.
4. Confirm that:
   - The object home page loads successfully.
   - Users can create new records.
   - Existing records can be viewed and managed.

The successful appearance of the **AI Lead Predictions** tab confirms that the tab configuration has been completed correctly.

---

## 8. Outcome

The custom tab was successfully configured and integrated into the Salesforce application. This enables users to easily access and manage AI Lead Prediction records from the Salesforce navigation menu, improving usability and streamlining lead management activities within the AI-Powered Lead Generation System.
