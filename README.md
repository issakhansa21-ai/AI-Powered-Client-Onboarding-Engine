# 🚀 AI-Powered Client Onboarding Automation  
**(n8n + Calendly + Airtable + OpenAI + Gmail)**

This project is a fully automated onboarding workflow built with **n8n**. It connects Calendly, Airtable, OpenAI, and Gmail to streamline the entire client intake process — from booking → CRM → personalized confirmation email.

## 📌 Overview
This workflow eliminates repetitive manual tasks and ensures every new client receives a fast, smooth, and professional onboarding experience. Once a call is booked on Calendly, the system automatically validates the booking, processes the client data, stores it in Airtable, generates a personalized message using AI, and sends the confirmation email instantly.

## ⚙️ Features

### 🔹 Calendly Trigger
Detects new bookings automatically via Calendly Webhooks.

### 🔹 Call Type Filtering
Runs only when the event type is “Onboarding”.

### 🔹 Data Structuring (Set Node)
Extracts and formats:
- Client Name  
- Client Email  
- Client Needs  
- Meeting Time  
- Meeting Link  

### 🔹 Airtable CRM Integration
Stores the client data in Airtable as a new CRM record.

### 🔹 AI Personalization (OpenAI)
Generates a personalized onboarding confirmation message using the client’s details.

### 🔹 Automatic Email Delivery (Gmail)
Sends the final message directly to the client’s inbox.

## 🧩 Tech Stack
- n8n  
- Calendly Webhooks  
- Airtable API  
- OpenAI Message Model  
- Gmail API  

## 📂 Workflow JSON
The full workflow file is included in this repository as:  
workflow.json

Import it into n8n using:
n8n → Settings → Import from File

## 🛠️ How It Works (Step-by-Step)
1. A client books an onboarding call on Calendly.  
2. Calendly sends a webhook event to n8n.  
3. n8n checks if the event type is “Onboarding”.  
4. Client data (name, email, booking info, etc.) is extracted and cleaned.  
5. A new record is created in Airtable.  
6. OpenAI generates a personalized email message.  
7. Gmail sends the confirmation email automatically.

## 📸 Screenshots
### n8n Workflow  

<img width="1920" height="905" alt="image 2" src="https://github.com/user-attachments/assets/3ba3a853-8dae-4a2b-a6e1-1bc2270964d6" />


### Airtable Record  

<img width="1920" height="902" alt="image 3 " src="https://github.com/user-attachments/assets/ce842435-9be5-4a40-bcbf-34c748c570d5" />


### Automated Email  

<img width="1920" height="827" alt="Image 4" src="https://github.com/user-attachments/assets/967f7cc7-993b-4d7d-a234-94393f77cfb2" />


## 🔗 Importing the Workflow
1. Clone or download this repository  
2. Open your n8n instance  
3. Go to Settings → Import  
4. Upload the file: workflow.json  
5. Add your credentials:
   - Calendly Webhook URL  
   - Airtable API Key + Base ID  
   - OpenAI API Key  
   - Gmail OAuth Credentials  

## 💡 Customization
You can easily customize:
- Trigger conditions  
- Email template  
- CRM fields  
- AI tone and length  
- Additional automation steps  

You can also expand this into a full onboarding system (reminders, questionnaires, contracts, etc.).

## 🤝 Need Help?
If you’d like help customizing this workflow or integrating it into a larger automation system, feel free to reach out.
