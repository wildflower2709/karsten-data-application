Inventory Request Power App + Automated Notification Flow

Status: Completed / In Progress
Tools: Power Apps, Power Automate, SharePoint / Excel / Dataverse

📌 Project Overview

This project demonstrates my ability to build functional low-code applications using Microsoft Power Apps and automate workflows using Power Automate.

It simulates an Inventory Request System where employees can request items, and managers automatically receive notifications for approval.

🎯 Objectives

Build a user-friendly Canvas App to submit and track inventory requests.

Connect app to a backend data source (SharePoint List / Excel / Dataverse).

Use Power Automate to trigger:

Email notifications

Status updates

Approvals

Document connectors and app logic.

📱 Power App Features

Submit a new inventory request

Dropdown selections for item type, quantity, department

Validation rules

A “My Requests” screen that shows request history

Manager view for approvals (optional)

🔁 Power Automate Flow Features

Trigger: New item added to SharePoint / Excel

Action 1: Send email to manager

Action 2: Write approval decision back to list

Action 3: Notify requestor automatically

🛠️ Connectors Used

Office 365 Outlook

SharePoint

Power Apps trigger connector

Excel Online (optional)

📂 Data Structure Example
Column	Type	Description
RequestID	Number	Unique ID
ItemName	Text	Item requested
Quantity	Number	Requested quantity
Status	Choice	Pending / Approved / Rejected
Requestor	Person	Submitted by
DateCreated	Date	When submitted
📸 Screenshots

(Add screenshots of your app screens here)

▶️ Demo Video (Optional)

Link: Add Google Drive / YouTube link

📥 How to Use

Import the app package

Update SharePoint/Excel connection

Test submission form

Trigger the flow

💡 Future Enhancements

Add role-based access control

Add thumbnail images for inventory items

Add push notifications

Add Power BI README
