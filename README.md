💊 AI-Based Pharmacy Management System (with Twilio Alert)
The Pharmacy Management System in the AI-enabled Smart Clinic is designed to automate and streamline medicine inventory, stock monitoring, and alerting, ensuring the continuous availability of essential drugs for patients. It operates intelligently by combining a real-time database, automated stock control, and Twilio-powered SMS alerts.

✅ Key Features
Medicine Inventory Management

Uses an SQLite database to store and manage medicine records.

Each entry includes:

Medicine name

Current stock level

Medicine ID (auto-generated)

Admins can add, update, or remove medicines as needed.

Stock Monitoring & Refill Management

Every time a medicine is added or updated, the system checks the stock level.

If stock falls below a defined critical threshold (e.g., 10 units), the system flags it as low.

Automated Twilio Alert System

A Twilio SMS alert is sent to the admin’s mobile number when any medicine is detected to be low in stock.

The message includes the medicine name and remaining quantity.

This helps prevent stockouts, especially for lifesaving or high-demand drugs.

📨 Sample SMS:
sql
Copy
Edit
Scalability & Integration

Easily expandable for hundreds of medicines.

Can be integrated with:

Doctor Prescription Analyzer (auto-deduct from stock)

Patient treatment logs

Billing and discharge modules

🔐 Security & Configuration
Sensitive details like Twilio credentials (SID, Auth Token, phone numbers) are stored in a separate secure config file (twilio_config.py).

Alerts are controlled to avoid false notifications (only trigger when genuinely low).

<img width="1440" alt="image" src="https://github.com/user-attachments/assets/e6f9aea9-47ff-45c0-aa96-96367e5cb700" />

<img width="1434" alt="image" src="https://github.com/user-attachments/assets/4f681020-eccf-4146-96a5-fe87b5a7cd59" />

<img width="1440" alt="image" src="https://github.com/user-attachments/assets/4a4ed393-3f0b-44f3-92ab-374d6c95888d" />
