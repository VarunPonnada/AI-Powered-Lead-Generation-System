# Fields and Relationships
## AI-Powered Lead Generation System

## Overview

Fields define the information stored within an object in Salesforce. Each field represents a specific attribute of a record, such as Lead Score, Lead Category, Product Interest, or AI Summary. Custom fields extend the functionality of standard Salesforce objects by allowing organizations to store project-specific information.

For the AI-Powered Lead Generation System, custom fields are created in the **Lead** object to capture AI-generated insights and classify leads effectively.

---

# Custom Fields Created

| Field Label | API Name | Data Type |
|-------------|----------|-----------|
| Lead Score | Lead_Score__c | Number |
| Lead Category | Lead_Category__c | Picklist (Hot, Warm, Cold) |
| Product Interest | Product_Interest__c | Picklist (Training, Consulting, Certification) |
| AI Summary | AI_Summary__c | Long Text Area |

---

# Steps to Create Custom Fields

## 1. Open Salesforce Setup

- Log in to Salesforce.
- Click the **⚙️ Gear** icon.
- Select **Setup**.

---

## 2. Open Object Manager

- Click **Object Manager** from the top navigation.
- Search for and select the **Lead** object.

---

## 3. Open Fields & Relationships

- In the left navigation panel, click **Fields & Relationships**.
- Click **New** to create a custom field.

---

# Field 1: Lead Score

### Data Type
**Number**

### Configuration

| Property | Value |
|----------|-------|
| Field Label | Lead Score |
| API Name | Lead_Score__c |
| Length | 18 |
| Decimal Places | 0 |

### Steps

1. Select **Number**.
2. Enter the field details.
3. Click **Next**.
4. Grant field visibility to the required profiles.
5. Add the field to page layouts.
6. Click **Save**.

---

# Field 2: Lead Category

### Data Type
**Picklist**

### Configuration

| Property | Value |
|----------|-------|
| Field Label | Lead Category |
| API Name | Lead_Category__c |

### Picklist Values

- Hot
- Warm
- Cold

### Steps

1. Select **Picklist**.
2. Choose **Enter values, with each value separated by a new line**.
3. Enter the picklist values.
4. Click **Next**.
5. Configure field-level security.
6. Add the field to page layouts.
7. Click **Save**.

---

# Field 3: Product Interest

### Data Type
**Picklist**

### Configuration

| Property | Value |
|----------|-------|
| Field Label | Product Interest |
| API Name | Product_Interest__c |

### Picklist Values

- Training
- Consulting
- Certification

### Steps

1. Select **Picklist**.
2. Enter the product interest values.
3. Click **Next**.
4. Configure field visibility.
5. Add the field to page layouts.
6. Click **Save**.

---

# Field 4: AI Summary

### Data Type
**Long Text Area**

### Configuration

| Property | Value |
|----------|-------|
| Field Label | AI Summary |
| API Name | AI_Summary__c |
| Length | 32768 |
| Visible Lines | 8 |

### Steps

1. Select **Long Text Area**.
2. Enter the field details.
3. Click **Next**.
4. Configure field-level security.
5. Add the field to page layouts.
6. Click **Save**.

---

# Verification

After creating all fields:

1. Open **Lead → Fields & Relationships**.
2. Verify the following custom fields are available:

- Lead Score
- Lead Category
- Product Interest
- AI Summary

3. Confirm that each field has the correct data type and API name.

---

# Outcome

The Lead object is successfully extended with custom fields that support AI-driven lead qualification. These fields enable lead scoring, categorization, product preference tracking, and AI-generated summaries, providing the foundation for intelligent lead management within the AI-Powered Lead Generation System.
