# Lab 1: Accelerate Purchase Order Review with Copilot in Dynamics 365 Business Central

**Lab Objective**

This lab is designed to help participants understand how Microsoft
Copilot can be used within Dynamics 365 Business Central to improve
efficiency in purchasing-related tasks. Throughout this lab, you will
work in a Business Central trial environment and explore Copilot
features such as data analysis, intelligent autofill, and conversational
insights. The lab focuses specifically on accelerating the review and
analysis of purchase orders using Copilot capabilities.

By completing this lab, participants will gain hands-on experience with
Copilot in real business scenarios and understand how AI-driven
assistance can support day-to-day purchasing operations.

## Exercise 1: Activate a Business Central Trial

In this exercise, you will activate a free trial environment for
Dynamics 365 Business Central. This environment will be used for all
subsequent exercises in this lab.

1.  Open your edge browser and navigate to
    +++<https://www.microsoft.com/en-us/dynamics-365/products/business-central>+++
    Microsoft Dynamics 365 Business Central product page.

2.  On the page, locate and click the **Try for free** button. This will
    initiate the trial activation process.

    ![](./media/image1.png)

3.  You will be prompted to enter your **Admin Tenant ID**. Enter the
    tenant ID associated with your Admin Tenant ID and click **Next** to
    continue.

    ![](./media/image2.png)

4.  Click the **Sign in** button to proceed to authentication.

    ![](./media/image3.png)

5.  If required, enter the administrator password and click **Sign in**
    again to confirm your credentials.

    ![](./media/image4.png)

6.  On the setup screen, provide the required information:

    - Select your **Country/Region** from the dropdown list

    - Enter your **Job Title** to indicate your role

    - Enter a valid **Business Phone Number**

7.  After completing the details, click **Get started** to activate the
    Business Central trial.

    ![](./media/image5.png)

8.  When prompted with optional setup steps, click **Skip and go to
    Business Central** to proceed directly to the application.

9.  Click **Get started** again to finalize the setup process.

    ![](./media/image6.png)

10. If a survey page appears, select **Skip survey** to bypass it.

    ![](./media/image7.png)

11. Once the process is complete, you will be redirected to the
    **Business Central home page**, confirming that your trial
    environment has been successfully activated and is ready for use.

    ![](./media/image8.png)

    ![](./media/image9.png)

    ![](./media/image10.png)

    ![](./media/image11.png)

    ![](./media/image12.png)

## Exercise 2: Create a Sandbox environment

Note: When a Business Central trial is activated, a Production
environment is automatically created and available for use. However, in
the current Production environment, some demo data required for upcoming
labs is not available. To ensure consistency and availability of
required demo data for future lab exercises, sandbox environments are
created using a previous release version specifically for lab guide
purposes.

1.  From the top bar of Business Central, click Settings, and then
    select Admin Center. The Business Central Admin Center opens in a
    new browser tab.

    ![](./media/image13.png)

2.  From the top menu, click New to start creating a new environment.

    ![](./media/image14.png)

3.  In the Create environment page, enter the following values:

    - Name: cronus_sandbox

    - Type: Sandbox

    - Country: United States (US)

    - Version: 26.0

4.  After entering the details, click Create. The environment creation
    process begins and the status shows that the environment is being
    configured.

    ![](./media/image15.png)

5.  While the sandbox environment is being created, select the
    Production environment from the environment list.

    ![](./media/image16.png)

    ![](./media/image17.png)

6.  Click the URL of the Production environment to open it.

    ![](./media/image18.png)

7.  You are redirected to the Business Central Production home page,
    confirming that the Production environment is accessible while the
    sandbox is provisioning.

    ![](./media/image19.png)

## Exercise 3: Verify Copilot and Agent Capabilities

In this exercise, you will verify that Copilot and agent capabilities
are enabled in your Business Central environment. These capabilities
allow Copilot to provide intelligent assistance throughout the
application.

1.  From the Business Central home page, press **Alt + Q** on your
    keyboard to open the **Tell me what you want** search bar.

2.  In the search field, type +++**Copilot & agent capabilities**.+++

3.  From the search results, select **Copilot & agent capabilities**.

    ![](./media/image20.png)

4.  Review the settings displayed on the page.

5.  In most trial environments, agent capabilities are enabled by
    default. You may review the available options to understand the
    scope of Copilot features. For the purpose of this lab, do **not**
    activate or deactivate any options.

    ![](./media/image21.png)

6.  Copilot and agent capabilities are confirmed to be active and
    available for use in subsequent exercises.

7.  Navigate to the business central home page, press the Alt + Q button
    on key board and enter +++Contoso Demo Tool+++ in the field, then
    select the option **Contoso Demo Tool.**

    ![](./media/image22.png)

8.  Click on the **Generate** button at the top and click on the **Yes**
    to confirm.

    ![](./media/image23.png)

9.  Press OK to complete the demo data setup.

    ![](./media/image24.png)

    ![](./media/image25.png)

## Exercise 4: Analyze Purchase Order Data Using Copilot

In this exercise, you will use Copilot to analyze purchase order data
directly from a list page. This demonstrates how Copilot can quickly
generate insights without manual filtering or calculations.

1.  Return to the **Business Central home page**.

2.  From the top navigation menu, select **Purchasing**.

3.  Click **Purchase Orders** to open the list of existing purchase
    orders.

    ![](./media/image26.png)

4.  On the Purchase Orders list page, locate and click the **Copilot
    icon** at the top of the list.

5.  From the Copilot menu, select **Analyze list**.

    ![](./media/image27.png)

6.  In the Copilot analysis window, enter the following prompt:

> +++**Show released status entries+++**

7.  Click **Generate** to allow Copilot to analyze the data.

    ![](./media/image28.png)

8.  Observe the generated analysis, which displays purchase orders
    filtered by released status.

    ![](./media/image29.png)

9.  At the bottom of the analysis window, locate the **Add more
    details** field.

10. Enter the following text:

> +++**Sort by amount+++**

11. Press **Enter** or click **Execute**.

    ![](./media/image30.png)

12. Copilot updates the analysis and sorts the purchase orders based on
    their values. Click on the **keep it** to save the changes.

    ![](./media/image31.png)

13. Navigate to the **Analysis1** sheet. Click the **Copilot icon**
    again and select **Create new analysis**.

    ![](./media/image32.png)

14. In the prompt area, click **Prompt options**.

15. Select **Add structure**, then choose **Group by**.

    ![](./media/image33.png)

16. After the group by statement, type:

> +++\[**average amount per vendor name\]+++**

17. Click **Generate** to run the analysis.

    ![](./media/image34.png)

18. Review the grouped results showing average purchase order amounts
    per vendor.

19. Click **Keep it** to save the analysis for future reference.

    ![](./media/image35.png)

20. A saved Copilot-generated analysis grouped by vendor, displaying
    average purchase order amounts.

## Exercise 5: Autofill Purchase Order Fields with Copilot (Preview)

In this exercise, you will experience how Copilot assists in
automatically filling in fields while creating a purchase order,
reducing manual data entry.

**Create a New Purchase Order**

1.  Navigate back to the **Business Central home page**.

2.  Select **Purchasing** from the top menu.

3.  Click **Purchase Orders**.

    ![](./media/image36.png)

4.  Click turn off the analysis mode and click on **+ New** to create a
    new purchase order.

    ![](./media/image37.png)

5.  In the **Vendor Name** field, open the dropdown list.

6.  Select **Graphic Design Institute**.

7.  Business Central automatically fills in vendor-related information
    such as address, payment terms, and posting groups.

    ![](./media/image38.png)

8.  Move your cursor to the **Your Reference** field.

9.  Hover over the field and click the **Autofill** option.

    ![](./media/image39.png)

10. Review the suggested or automatically populated content provided by
    Copilot.

11. In the Copilot suggestion panel displayed in the top-right corner,
    click **Got it**.

    ![](./media/image40.png)

12. Click the **Details (information) icon** next to the **Your
    Reference** field.

13. Review the explanation and suggestions provided by Copilot.

14. Choose **Keep** or **Change** depending on your business
    requirement.

    ![](./media/image41.png)

15. The purchase order fields are intelligently populated with Copilot
    assistance.

## Exercise 6: Chat with Copilot (Preview)

In this exercise, you will interact with Copilot using natural language
to retrieve insights and navigate business data.

1.  Return to the **Business Central home page**.

2.  Click the **Copilot icon** located at the top of the screen.

    ![](./media/image42.png)

3.  In the Copilot chat window, type the following query:

> +++Show me the top five high-value purchase orders+++

4.  Press **Enter** or click the **Execute** icon.

    ![](./media/image43.png)

5.  Review the list of purchase orders suggested by Copilot.

6.  Select the first purchase order from the list to explore further.

    ![](./media/image44.png)

7.  Verify the purchase order details displayed on the screen.

    ![](./media/image45.png)

8.  At the bottom of the Copilot window, click **View prompt**.

9.  Review the prompt guidance that helps structure effective queries.

10. Click **Find**, then select **Look up**.

    ![](./media/image46.png)

    ![](./media/image47.png)

11. Enter the following text after look up:

> +++**Vendor number 30000+++**

12. Press **Enter** or click **Execute**.

    ![](./media/image48.png)

13. Copilot retrieves and displays information related to vendor number
    30000.

    ![](./media/image49.png)

14. Click the vendor link to view complete vendor details.

    ![](./media/image50.png)

## Lab Completion

You have successfully completed this lab. You now understand how Copilot
can accelerate purchase order review, analysis, and data entry in
Dynamics 365 Business Central, enabling faster and more informed
business decisions.
