# Lab 6: Vendor Invoice Automation for SMB Finance Teams with Copilot in Dynamics 365 Business Central

## Overview

In this lab, you will explore how Copilot enhances vendor invoice processing in Dynamics 365 Business Central for small and medium-sized finance teams. The lab walks through configuring the **Payables Agent**, setting up an email inbox for receiving vendor invoices, and using Copilot to automatically create, review, and post purchase documents.

You will also gain hands-on experience reviewing invoice data, making necessary adjustments, and using Copilot to manage number series. By the end of this lab, you will have a clear understanding of how invoice automation works end to end within Business Central, and how Copilot reduces manual effort while you keep control over financial transactions.

## Objectives

- Activate and configure the Payables Agent, including its mailbox.
- Send a vendor invoice by email and review it in Business Central.
- Review, adjust, finalize, and post a Copilot-generated purchase invoice.
- Create and modify number series using Copilot.
- Prepare number series for the next year with Copilot.

## Prerequisites

- Access to the Business Central environment configured in **Lab 1**, with admin tenant credentials.
- A personal email account (for example, Outlook.com) to act as the vendor.
- The file **Fabrikam Invoice US D365F** in the **C:\labfiles** folder.

## Estimated Time

**45 minutes**

> [!NOTE]
> Text shown as +++sample text+++ can be typed or copied directly into the lab environment. Copilot and agent responses are AI-generated, so your results may differ slightly from the screenshots.

---

## Exercise 1: Configure the Payables Agent

In this exercise, you will activate the Payables Agent, connect a mailbox, and update its settings.

### Task 1: Activate the Payables Agent

1. Navigate to the Business Central sign-in page and sign in with the admin tenant:

    +++https://www.microsoft.com/en-us/dynamics-365/products/business-central/sign-in+++

    ![](./media/image1.png)

2. Select **Payables Agent** from the top menu to begin configuring automated invoice processing.

    ![](./media/image2.png)

3. Select **Activate** to start enabling the agent.

    ![](./media/image3.png)

4. Turn **On** the **Activate** toggle so the Payables Agent can receive and process vendor invoices.

    ![](./media/image4.png)

### Task 2: Configure the Mailbox for the Payables Agent

1. Select the right-side arrow on the Payables Agent card.

    ![](./media/image5.png)

2. In the **Mailbox** section, select the **horizontal ellipsis (⋯)** to configure how invoices will be received.

    ![](./media/image6.png)

3. Select **Next** to assign an email account to the agent.

    ![](./media/image7.png)

4. Select **Current user**, allowing the agent to use the signed-in user's mailbox for receiving invoices, and then select **Next**.

    ![](./media/image8.png)

5. Select **Next** again to confirm the mailbox setup.

    ![](./media/image9.png)

6. Select **Finish** to complete the mailbox configuration.

    ![](./media/image10.png)

7. Verify that **Current user** appears in the **Email accounts** section, and then select **OK**.

    ![](./media/image11.png)

### Task 3: Review and Update Payables Agent Settings

1. Select the **right-arrow (>)** icon to access additional configuration options.

    ![](./media/image12.png)

2. Review the **Get sample invoice** section to understand how invoices are interpreted during processing.

3. In the **Document processing** section, ensure **Review email** is turned **On** so incoming emails can be reviewed before document creation.

4. Select **Update** to save the Payables Agent configuration.

    ![](./media/image13.png)

5. Accept the terms and conditions by selecting **I accept**.

    ![](./media/image14.png)

> **✅ Result:** The Payables Agent is active and connected to the current user's mailbox.

---

## Exercise 2: Process a Vendor Invoice with the Payables Agent

In this exercise, you will send a vendor invoice by email and use the Payables Agent and Copilot to create, review, and post the purchase invoice.

### Task 1: Send a Vendor Invoice Email

1. Open a new browser tab and navigate to Outlook:

    +++https://outlook.live.com/mail/+++

2. Sign in using a **personal email account** to simulate a vendor sending an invoice.

    ![](./media/image15.png)

> [!WARNING]
> Send the email **from** your personal account **to** the admin tenant email address configured for the Payables Agent. Do not send it from the tenant mailbox itself, or the vendor scenario will not be simulated correctly.

3. Create a new email addressed to the admin tenant email address configured for the Payables Agent.

4. Enter the following subject:

    +++Invoice+++

5. Enter the following email body:

    +++Dear Team, Please find attached the Fabrikam invoice for your review and further processing. Kindly verify the details and let us know if any clarification or correction is required from our end. Thank you for your support.+++

6. Attach the **Fabrikam Invoice US D365F** file from the **C:\labfiles** folder, and then send the email to start invoice processing.

    ![](./media/image16.png)

### Task 2: Review the Incoming Invoice in Business Central

1. Return to the **Business Central** portal once the email is sent.

> [!NOTE]
> The agent checks the mailbox periodically, so it can take a few minutes for the new request to appear. Refresh the page if needed.

2. The Payables Agent detects the incoming email and creates an **e-Document** request. Open the most recent request.

    ![](./media/image17.png)

3. Select **Review** to validate the email content.

    ![](./media/image18.png)

4. Select **View PDF** to examine the invoice document.

    ![](./media/image19.png)

5. Close the document, and then select **Continue** to allow Copilot to create a draft purchase document.

    ![](./media/image20.png)

    ![](./media/image21.png)

### Task 3: Review and Update the Purchase Document Draft

1. Wait while Copilot prepares the purchase document draft.

2. Once the draft is ready, select **Review** to examine the generated details.

    ![](./media/image22.png)

3. Scroll down to the **Total Tax** section and update the tax value to +++120+++.

    ![](./media/image23.png)

    ![](./media/image24.png)

4. Select **Continue** to move forward with the updated draft.

    ![](./media/image25.png)

### Task 4: Finalize and Post the Purchase Invoice

1. Allow Copilot to finalize the draft based on the reviewed information.

2. Select **Finalize purchase draft** once the final version is available.

    ![](./media/image26.png)

3. Review the finalized document, and then select **Post**.

    ![](./media/image27.png)

> [!WARNING]
> Posting creates ledger entries that cannot be edited. Verify the vendor, lines, and totals before you confirm.

4. Confirm the posting by selecting **Yes**.

    ![](./media/image28.png)

5. Select **Yes** again to view the posted document.

    ![](./media/image29.png)

> **✅ Result:** You have processed a vendor invoice received by email from draft to posted purchase invoice.

---

## Exercise 3: Manage Number Series with Copilot

In this exercise, you will review existing number series, then use Copilot to create, modify, and prepare number series for the next year.

### Task 1: Review Existing Number Series

1. Navigate to the **Business Central home page**.

2. Select **Purchasing** from the top menu, and then open **Purchase Orders** to review the automatically assigned order numbers.

    ![](./media/image30.png)

    ![](./media/image31.png)

3. Return to the home page, press **Alt + Q**, type +++Purchases & Payables Setup+++, and select **Purchases & Payables Setup**.

    ![](./media/image32.png)

4. Notice that the **IRS 1096 Form No.** series is not available in the setup. Select **Back** at the top.

    ![](./media/image33.png)

5. Press **Alt + Q**, type +++Number Series+++, and open the **Number Series** page to view how document numbers are generated.

    ![](./media/image34.png)

### Task 2: Create a Number Series Using Copilot

1. On the **Number Series** page, select **Generate** to let Copilot suggest changes.

    ![](./media/image35.png)

2. Enter the following prompt, and then select **Generate**:

    +++Create a number series for the IRS 1096 Form no. series for the current year+++

    ![](./media/image36.png)

3. Select **Keep it** to save the number series.

    ![](./media/image37.png)

4. Press **Alt + Q**, type +++Purchases & Payables Setup+++, and select **Purchases & Payables Setup**.

    ![](./media/image38.png)

5. Scroll down to confirm that the **IRS 1096** number series has been created, and then select **Back**.

    ![](./media/image39.png)

### Task 3: Modify a Number Series Using Copilot

1. Select the **Generate** button at the bottom of the page.

    ![](./media/image40.png)

2. Enter the following prompt to modify the **Sales Order** number series, and then select **Generate**:

    +++Change the [Sales Order] number to [SORD- 1099]+++

    ![](./media/image41.png)

3. Review the suggested changes, and then select **Keep it** to apply them.

    ![](./media/image42.png)

    ![](./media/image43.png)

> [!IMPORTANT]
> Changing a number series affects all new documents of that type. In a live company, confirm such changes with your finance team before applying them.

### Task 4: Prepare Number Series for the Next Year

1. Select **Generate** again to explore additional Copilot capabilities.

    ![](./media/image44.png)

2. Open the **Prompt guidance**, select **Prepare for next year**, and then select **Prepare number series for the next year**.

    ![](./media/image45.png)

3. Select **Generate**.

    ![](./media/image46.png)

4. Review the generated number series, and then select **Keep it** to save the changes.

    ![](./media/image47.png)

> **✅ Result:** You have used Copilot to create, modify, and roll forward number series in Business Central.

---

## Summary

By completing this lab, you have configured the Payables Agent and used Copilot to automate the processing of vendor invoices received by email. You reviewed incoming documents, validated and adjusted purchase details, finalized and posted invoices, and explored how Copilot can help manage number series efficiently. This lab demonstrates how Copilot helps finance teams streamline accounts payable processes, improve accuracy, and reduce manual intervention while retaining full visibility and control within Dynamics 365 Business Central.

## Key Takeaways

- The Payables Agent monitors a mailbox and turns vendor invoice emails into e-documents and draft purchase invoices.
- Review steps let you check and correct data before a document is finalized and posted.
- Copilot can create, modify, and roll forward number series from plain-language prompts.
- Always review AI-generated content, as Copilot and agent results may occasionally be incomplete or incorrect.
