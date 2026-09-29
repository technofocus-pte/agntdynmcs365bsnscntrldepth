# Copilot in Dynamics 365 Business Central – Hands-on Lab Series

## Overview

This repository contains eight hands-on lab guides that show how Microsoft Copilot and AI agents in Dynamics 365 Business Central help with everyday purchasing, sales, finance, and inventory work. Each lab walks you step by step through a real business scenario in the **CRONUS** demo company, with screenshots for every step.

## Labs

| Lab | Title | Exercises | Estimated Time |
|:---:|-------|:---------:|:--------------:|
| 1 | [Accelerate Purchase Order Review with Copilot in Dynamics 365 Business Central](./Lab%201/Lab%201%20-%20Accelerate%20Purchase%20Order%20Review%20with%20Copilot%20in%20Dynamics%20365%20Business%20Central.md) | 5 | 45 minutes |
| 2 | [Improve Order Fulfillment and Customer Satisfaction using Suggest Substitute Items and Summarize Records with Copilot](./Lab%202/Lab%202%20-%20Improve%20Order%20Fulfillment%20and%20Customer%20Satisfaction%20using%20Suggest%20substitute%20items%20and%20summarize%20records%20with%20Copilot.md) | 2 | 20 minutes |
| 3 | [Map E-Documents to Purchase Order Lines with Copilot in Dynamics 365 Business Central](./Lab%203/Lab%203%20-%20Map%20e-documents%20to%20purchase%20order%20lines%20with%20Copilot%20in%20Dynamics%20365%20Business%20Central.md) | 2 | 25 minutes |
| 4 | [Creating and Enhancing Item Marketing Text with Copilot in Business Central](./Lab%204/Lab%204%20-%20Creating%20and%20Enhancing%20Item%20Marketing%20Text%20with%20Copilot%20in%20Business%20Central.md) | 2 | 20 minutes |
| 5 | [Analyze Open Sales Invoices Using Copilot Chat and Analysis Assist in Dynamics 365 Business Central](./Lab%205/Lab%205%20-%20Analyze%20Open%20Sales%20Invoices%20Using%20Copilot%20Chat%20and%20Analysis%20Assist.md) | 4 | 30 minutes |
| 6 | [Vendor Invoice Automation for SMB Finance Teams with Copilot in Dynamics 365 Business Central](./Lab%206/Lab%206%20-%20Vendor%20Invoice%20Automation%20for%20SMB%20Finance%20Teams%20with%20Copilot%20in%20Dynamics%20365%20Business%20Central.md) | 3 | 45 minutes |
| 7 | [Automating Sales Order Capture for Faster Order Processing with the Sales Order Agent](./Lab%207/Lab%207%20-%20Automating%20Sales%20Order%20Capture%20for%20Faster%20Order%20Processing%20with%20the%20Sales%20Order%20Agent.md) | 2 | 30 minutes |
| 8 | [Configure and Activate Expense Agent for Automated Expense Processing in Dynamics 365 Business Central](./Lab%208/Lab%208%20-%20Configure%20and%20Activate%20Expense%20Agent%20for%20Automated%20Expense%20Processing.md) | 2 | 30 minutes |

> [!IMPORTANT]
> Complete **Lab 1** first. It activates the Business Central trial, verifies Copilot and agent capabilities, and generates the demo data used by the later labs.

## What You Will Learn

- **Copilot features:** Analyze list and Analysis Assist, Autofill, Copilot Chat and the prompt guide, substitute item suggestions, record summaries, e-document line mapping, marketing text drafting, and number series generation.
- **AI agents:** the Payables Agent (vendor invoices), the Sales Order Agent (customer inquiries and quotes), and the Expense Agent (expense reports).

## Prerequisites

- Admin tenant credentials for Dynamics 365 Business Central.
- Microsoft Edge or another supported browser.
- A personal email account (for example, Outlook.com) for the agent labs (Labs 6 and 7).
- The file **Fabrikam Invoice US D365F** in **C:\labfiles** (Lab 6).
- A **cronus_sandbox** environment (Lab 3).
- A Microsoft Exchange license for the signed-in user (Lab 8).

## Repository Structure

```
Business_Central_Copilot_Lab_Guides/
├── README.md
├── Lab 1/
│   ├── Lab 1 - <full lab title>.md
│   └── media/
│       ├── image1.png
│       └── ...
├── Lab 2/
│   ├── Lab 2 - <full lab title>.md
│   └── media/
└── ... (Lab 3 to Lab 8 follow the same pattern)
```

Each lab folder contains one markdown guide and a `media` folder with all of its screenshots. Images are referenced with relative paths, for example `![](./media/image1.png)`, so keep each `.md` file and its `media` folder together.

## Lab Guide Format

Every guide follows the same structure: Overview, Objectives, Prerequisites, Estimated Time, Exercises (split into Tasks), a Result checkpoint at the end of each exercise, Summary, and Key Takeaways.

### Conventions

| Element | Meaning |
|---------|---------|
| `+++text+++` | A value to type or copy into the lab environment, such as a prompt, URL, or code. |
| **Bold text** | A UI element to select, such as a button, field, page, or menu. |
| `> **✅ Result:**` | A checkpoint confirming what you accomplished in the exercise. |
| `> [!NOTE]` | Helpful background information. |
| `> [!TIP]` | A suggestion to work faster or get better results. |
| `> [!IMPORTANT]` | Information you need to complete the lab correctly. |
| `> [!WARNING]` | An action that can cause errors or unwanted changes if done incorrectly. |

> [!NOTE]
> Copilot and agent responses are AI-generated, so your results may differ slightly from the screenshots. Always review AI-generated content before saving or posting.

## Total Duration

Approximately **4 hours** to complete all eight labs.
