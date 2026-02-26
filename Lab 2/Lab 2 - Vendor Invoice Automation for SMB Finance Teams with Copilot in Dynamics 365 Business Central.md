# Lab 2: Vendor Invoice Automation for SMB Finance Teams with Copilot in Dynamics 365 Business Central

**Introduction**

In this lab, participants will explore how Copilot enhances vendor
invoice processing in Dynamics 365 Business Central for small and
medium-sized finance teams. The lab walks through configuring the
Payables Agent, setting up an email inbox for receiving vendor invoices,
and using Copilot to automatically create, review, and post purchase
documents. Participants will also gain hands-on experience reviewing
invoice data, making necessary adjustments, and understanding how
Copilot assists in reducing manual effort while maintaining control over
financial transactions. By the end of this lab, participants will have a
clear understanding of how invoice automation works end to end within
Business Central.

## Task 1: Activate the Payables Agent

1.  Navigate to
    <https://www.microsoft.com/en-us/dynamics-365/products/business-central/sign-in>
    business central and sign in with the admin tenant.

> ![](./media/image1.png)

2.  Navigate to **Payables Agent** from the top menu to begin
    configuring automated invoice processing.

> ![](./media/image2.png)

3.  Click **Activate** to start enabling the agent.

> ![](./media/image3.png)

4.  Turn **On** the **Activate** toggle so the Payables Agent can
    receive and process vendor invoices.

> ![](./media/image4.png)

## Task 2: Configure the Mailbox for the Payables Agent

1.  In the **Mailbox** section, click the **horizontal ellipsis (⋯)** to
    configure how invoices will be received.

> ![](./media/image5.png)

2.  Click **Next** to assign an email account to the agent.

> ![](./media/image6.png)

3.  From the available options, select **Current user**, allowing the
    agent to use the signed-in user’s mailbox for receiving invoices,
    then click **Next**.

> ![](./media/image7.png)

4.  Click **Next** again to confirm the mailbox setup.

> ![](./media/image8.png)

5.  Click **Finish** to complete the mailbox configuration.

> ![](./media/image9.png)

6.  Verify that **Current user** appears in the **Email accounts**
    section and click **OK** to finalize the setup.

> ![](./media/image10.png)

## Task 3: Review and Update Payables Agent Settings

1.  Click the **right-arrow (\>)** icon to access additional
    configuration options.

> ![](./media/image11.png)

2.  Review the **Get sample invoice** section to understand how invoices
    are interpreted during processing.

3.  In the **Document processing** section, ensure **Review email** is
    turned **On** so incoming emails can be reviewed before document
    creation.

4.  Click **Update** to save the Payables Agent configuration.

> ![](./media/image12.png)

5.  Accept the terms and conditions by clicking **I accept** to proceed.

> ![](./media/image13.png)

## Task 4: Send a Vendor Invoice Email

1.  Open a new browser tab and navigate to
    [**https://outlook.live.com/mail/**](https://outlook.live.com/mail/).

2.  Sign in using a personal email account to simulate a vendor sending
    an invoice.

> ![](./media/image14.png)

3.  Create a new email and send it to the same admin tenant email
    address configured for the Payables Agent.

4.  Set the subject as **Invoice** and add the provided email content.

Dear Team,

Please find attached the **Fabrikam invoice** for your review and
further processing.

Kindly verify the details and let us know if any clarification or
correction is required from our end.

Thank you for your support.

5.  Attach the **Fabrikam Invoice US D365F** file from the C:\labfiles
    folder and send the email to initiate invoice processing.

> ![](./media/image15.png)

## Task 5: Review the Incoming Invoice in Business Central

1.  Return to the **Business Central** portal once the email is sent.

2.  Notice that the Payables Agent automatically detects the incoming
    email and creates an **e-Document** request. Open the most recent
    request.

> ![](./media/image16.png)

3.  Click **Review** to validate the email content.

> ![](./media/image17.png)

4.  Select **View PDF** to examine the invoice document.

> ![](./media/image18.png)

5.  Close the document and click **Continue** to allow Copilot to create
    a draft purchase document.

> ![](./media/image19.png)
>
> ![](./media/image20.png)

## Task 6: Review and Update the Purchase Document Draft

1.  Wait while Copilot prepares the purchase document draft.

2.  Once the draft is ready, click **Review** to examine the generated
    details.

> ![](./media/image21.png)

3.  Scroll down to the **Total Tax** section and update the tax value to
    **120**.

> ![](./media/image22.png)
>
> ![](./media/image23.png)

4.  Click **Continue** to move forward with the updated draft.

> ![](./media/image24.png)

## Task 7: Finalize and Post the Purchase Invoice

1.  Allow Copilot to finalize the draft based on the reviewed
    information.

2.  Click **Finalize purchase draft** once the final version is
    available.

> ![](./media/image25.png)

3.  Review the finalized document and click **Post** to complete the
    transaction.

> ![](./media/image26.png)

4.  Confirm the posting by clicking **Yes.**

> ![](./media/image27.png)

5.  Click **Yes** again to view the posted document.

> ![](./media/image28.png)

## Task 8: Create and update Number Series

1.  Navigate to the **Business Central Home** page.

2.  Select **Purchasing** from the top menu and open **Purchase Orders**
    to review the automatically assigned order numbers.

> ![](./media/image29.png)
>
> ![](./media/image30.png)

3.  Navigate to the homage page, Press Alt + Q, enter Payable setup in
    the field, and select **Purchase & Payable** setup option.

> ![](./media/image31.png)

4.  Participant can see IRS 1096 Form no. series is not available in the
    setup. Click on the Back button at the top.

> ![](./media/image32.png)

5.  Press **Alt + Q**, search for **Number Series**, and open the
    **Number Series** page to view how document numbers are generated.

> ![](./media/image33.png)

## Task 9: Generate and Update Number Series Using Copilot

1.  From the **Number Series** page, click **Generate** to let Copilot
    suggest changes.

> ![](./media/image34.png)

2.  Enter the provided prompt and click **Generate**.

> +++Create a number series for the IRS 1096 Form no. series for the
> current year+++
>
> ![](./media/image35.png)

3.  Click on Keep it to save the number series.

> ![](./media/image36.png)

4.  Press Alt + Q and enter Payable setup, then select Purchases &
    payable setup option.

> ![](./media/image37.png)

5.  Scroll down and can see the IRS 1096 number series is created. Click
    on the back button from top.

> ![](./media/image38.png)

6.  Press the **Generate** button from the bottom.

> ![](./media/image39.png)

7.  Enter the provided prompt to modify the **Sales Order number
    series** and click **Generate**.

> +++Change the \[Sales Order\] number to \[SORD- 1099\]+++
>
> ![](./media/image40.png)

8.  Review the suggested changes and click **Keep it** to apply them.

> ![](./media/image41.png)
>
> ![](./media/image42.png)

**Task 10: Prepare Number Series for the Next Year**

1.  Click **Generate** again to explore additional Copilot capabilities.

> ![](./media/image43.png)

2.  Open the **Prompt guidance** and select **Prepare for next year**.

3.  Choose **Prepare number series for the next year**.

> ![](./media/image44.png)

4.  Click **Generate**.

> ![](./media/image45.png)

5.  Review the generated number series and click **Keep it** to save the
    changes.

> ![](./media/image46.png)

**Conclusion**

By completing this lab, participants have successfully configured the
Payables Agent and used Copilot to automate the processing of vendor
invoices received via email. They reviewed incoming documents, validated
and adjusted purchase details, finalized and posted invoices, and
explored how Copilot can assist in managing number series efficiently.
This lab demonstrates how Copilot helps finance teams streamline
accounts payable processes, improve accuracy, and reduce manual
intervention while retaining full visibility and control within Dynamics
365 Business Central.
