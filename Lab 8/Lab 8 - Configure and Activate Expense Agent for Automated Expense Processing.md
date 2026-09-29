# Lab 8: Configure and Activate Expense Agent for Automated Expense Processing in Dynamics 365 Business Central

## Overview

Processing employee expense reports by hand is slow and error-prone. Finance teams have to read every receipt, key in the amounts, check each line against company policy, and then chase approvers, all before an employee can be reimbursed.

The **Expense Agent** is a Microsoft-built AI agent in Dynamics 365 Business Central that takes over much of this work. It reads employee receipts, extracts the data, validates each entry against company policy, and routes the report for approval. Before it can do any of that, two things must be in place: the agent has to be activated and connected to an email account, and the company's expense master data (payment methods, categories, subcategories, groups, and locations) must be defined so that expenses can be classified and posted correctly.

In this lab, you will work in the **CRONUS USA, Inc.** demo company as an administrator. In Exercise 1, you will activate the Expense Agent and connect a Current User email account. In Exercise 2, you will review the expense payment methods, create a new **TRAINING** expense category with a **SKILL** expense group and a **COURSEFEE** subcategory, and add a new expense location for Switzerland.

## Objectives

- Activate the Expense Agent from the Tasks pane and switch it on.
- Set up a Current User email account so the agent can correspond with employees and approvers.
- Accept the Azure OpenAI terms and confirm that the agent is running.
- Use the **Tell me what you want to do** search to open expense setup pages.
- Create an expense category with a posting group, default payment method, expense group, and subcategory.
- Add a new expense location for a country or region.

## Prerequisites

- Access to a Dynamics 365 Business Central environment with the **CRONUS USA, Inc.** demo company.
- A user account with administrator permissions to configure agents and email accounts.
- A valid Microsoft Exchange license for the signed-in user, which the Current User email account requires.

## Estimated Time

**30 minutes**

> [!NOTE]
> Text shown as +++sample text+++ can be typed or copied directly into the lab environment. The Expense Agent uses AI, so screens and messages in your environment may differ slightly from the screenshots.

---

## Exercise 1: Activate and Configure the Expense Agent

In this exercise, you will activate the Expense Agent from the Tasks pane, switch it on from the Configure Expense Agent page, and complete the Set Up Email guide using the Current User account type, so that each person sends messages from their own sign-in account. You will then accept the Azure OpenAI terms and confirm that the agent is live.

### Task 1: Activate the Expense Agent

1. Sign in to Dynamics 365 Business Central. The Role Center for **CRONUS USA, Inc.** opens. In the top navigation bar, select the **Expense Agent (EA)** icon.

    ![](./media/image1.png)

2. The **Tasks** pane opens on the right and shows that the Expense Agent is ready to activate. Select **Activate**.

    ![](./media/image2.png)

3. The **Configure Expense Agent** page opens. Switch the **Active** toggle on.

    ![](./media/image3.png)

### Task 2: Set Up the Email Account

1. With the toggle on, the **Update** button becomes available. Select the next arrow (**>**) to the right of the agent card to move to the agent settings, locate **Enable sending email with receipts**, and select the ellipsis (**…**) next to it.

    ![](./media/image4.png)

2. The **Set Up Email** guide opens, because the agent needs an email account to communicate with employees and approvers. Read the welcome text and the privacy notice, and then select **Next**.

    ![](./media/image5.png)

3. Under **Specify the type of email account to add**, select **Current User** so that each user sends email from their own sign-in account, and then select **Next**.

    ![](./media/image6.png)

> [!WARNING]
> The **Current User** account type requires a valid Microsoft Exchange license for every user who sends email. Without it, the agent cannot send messages.

4. The **Current User Email Account** page explains that everyone will send email from their own account. Select **Next**.

    ![](./media/image7.png)

5. The account is added successfully. Leave **Set as default** switched on, keep **Rate Limit per Minute** at **30**, and select **Finish**.

    ![](./media/image8.png)

6. The **Email Accounts** list shows the new **Current User** account. Select **OK** to return to the agent setup.

    ![](./media/image9.png)

### Task 3: Apply the Settings and Accept the Terms

1. On the **Configure Expense Agent** page, select **Update** to apply the settings.

    ![](./media/image10.png)

2. The **Please review terms and conditions** dialog opens. Read the terms for Azure OpenAI, and then select **Agree**.

    ![](./media/image11.png)

3. Verify that the **Tasks** pane now shows **Expense Agent** as **Configured by** your administrator account. Tasks that need attention, and recent ongoing and completed tasks, will appear in this pane.

    ![](./media/image12.png)

> **✅ Result:** You have activated the Expense Agent, connected a Current User email account, and accepted the Azure OpenAI terms. The agent is now configured and running.

---

## Exercise 2: Set Up Expense Payment Methods, Categories, and Locations

Before the Expense Agent can process employee expense reports, Business Central needs master data that tells it how expenses should be classified and posted. **Payment methods** define who paid (the company, a credit card, or the employee). **Expense categories and subcategories** define what the expense was for and which posting group it maps to. **Expense locations** define where the expense was incurred.

In this exercise, you will review the standard expense payment methods, create a new TRAINING expense category with a COURSEFEE subcategory and a new SKILL expense group, and then add a new expense location for Switzerland.

### Task 1: Review Expense Payment Methods

1. On the Business Central home page, select the **Search** (magnifier) icon in the top navigation bar. In the **Tell me what you want to do** box, type:

    +++Expense Payment Methods+++

    Under **Go to Pages and Tasks**, select **Expense Payment Methods**.

    ![](./media/image13.png)

2. Review the three standard payment methods: **BANK** (Company Paid), **CARD** (Credit Card), and **CASH** (Employee Paid). These control how each expense is reimbursed.

    ![](./media/image14.png)

3. Select the **Back** arrow in the top-left corner to return to the home page.

    ![](./media/image15.png)

### Task 2: Create the TRAINING Expense Category

1. Select the **Search** icon again. In the **Tell me what you want to do** box, type:

    +++Expense Categories+++

    Under **Go to Pages and Tasks**, select **Expense Categories**.

    ![](./media/image16.png)

2. The **Expense Categories** list opens, showing the standard categories such as **AIRLINE**, **HOTELS**, and **MEALS**. Select **+ New** to create an additional expense category.

    ![](./media/image17.png)

3. On the **Expense Category** card, in the **Code** field, type:

    +++TRAINING+++

    ![](./media/image18.png)

4. In the **Description** field, type:

    +++Expenses for professional training and skills development, including course fees, certification and examination fees, workshops, seminars, and e-learning subscriptions. Excludes conferences, trade fairs, and exhibitions.+++

    ![](./media/image19.png)

> [!TIP]
> A clear, detailed description helps the Expense Agent decide which category a receipt belongs to. State what the category includes and what it excludes.

5. In the **Posting Description** field, type:

    +++Training and certification+++

    ![](./media/image20.png)

6. Open the **Posting Group** drop-down to see the available expense posting groups, and select **EXPENSE-OTHER**.

    ![](./media/image21.png)

7. Open the **Default Payment Method** drop-down, review the options (**BANK**, **CARD**, and **CASH**), and select **CARD**. Notice that **Reimbursement Type** is filled in automatically as **Credit Card**.

    ![](./media/image22.png)

### Task 3: Create the SKILL Expense Group

1. Open the **Expense Group** drop-down. The existing groups don't cover training, so select **+ New** to create one.

    ![](./media/image23.png)

2. In the **Select - Expense Groups** window, in the **Code** field of the new line, type:

    +++SKILL+++

    ![](./media/image24.png)

3. In the **Description** field, type the following, and then select **OK**:

    +++Training and certification+++

    ![](./media/image25.png)

4. Back on the Expense Category card, the **Expense Group** field now shows **SKILL**. Switch the **Refundable** toggle on so that this category can be reimbursed.

    ![](./media/image26.png)

### Task 4: Add the COURSEFEE Subcategory

1. In the action bar, select **Subcategories** to add detail lines.

    ![](./media/image27.png)

2. On the **Expense Subcategories** page, in the **Code** field, type:

    +++COURSEFEE+++

    In the **Description** field, type:

    +++Tuition and registration fees for professional training courses, workshops, and seminars attended for business purposes. Covers instructor-led, virtual, and self-paced course enrolment charges.+++

    ![](./media/image28.png)

3. In the **Posting Description** field, type:

    +++Course fee+++

    ![](./media/image29.png)

4. Select the **Refundable** checkbox for the subcategory, and then select the **Back** arrow.

    ![](./media/image30.png)

> [!IMPORTANT]
> If **Refundable** is not selected, expenses in this category or subcategory will not be reimbursed to employees.

5. On the **Expense Categories** list, scroll down to confirm that the new **TRAINING** category is saved, and then select the **Back** arrow to return to the home page.

    ![](./media/image31.png)

### Task 5: Add a New Expense Location

1. Select the **Search** icon. In the **Tell me what you want to do** box, type:

    +++Expense Locations+++

    Under **Go to Pages and Tasks**, select **Expense Locations**.

    ![](./media/image32.png)

2. Review the existing locations, and then select **+ New** to add another one.

    ![](./media/image33.png)

3. On the **Expense Location Card**, in the **No.** field, type:

    +++SWISS-ALL+++

    ![](./media/image34.png)

4. Open the **Country/Region Code** drop-down and select **Switzerland** (**CH**). Then, in the **Description** field, type:

    +++CH+++

    The card saves automatically, and the new Swiss location is ready to be used on expense reports.

    ![](./media/image35.png)

> **✅ Result:** You have reviewed the expense payment methods, created the TRAINING expense category with the SKILL expense group and the COURSEFEE subcategory, and added the SWISS-ALL expense location.

---

## Summary

In this lab, you took the Expense Agent in Dynamics 365 Business Central from switched off to fully operational. In Exercise 1, you activated the agent, connected a Current User email account so it can correspond with employees and approvers, and accepted the Azure OpenAI terms.

In Exercise 2, you gave the agent the master data it depends on. You reviewed the payment methods, built a TRAINING category with its SKILL expense group and COURSEFEE subcategory, and added a Swiss expense location. Together, these settings define who paid, what the expense was for, how it is posted, and where it happened.

The agent can now extract receipt data, validate it against these settings, and route expense reports for approval.

## Key Takeaways

- The Expense Agent must be activated and connected to an email account before it can process expense reports.
- The Current User email account type lets each person send messages from their own sign-in account.
- Expense payment methods, categories, subcategories, groups, and locations are the master data the agent uses to classify and post expenses.
- The **Tell me what you want to do** search is the quickest way to reach any setup page in Business Central.
- Always review the agent's output, as AI-generated results may occasionally be incomplete or incorrect.
