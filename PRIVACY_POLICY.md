# Privacy Policy for Self Audit Expense Tracker

**Effective Date:** March 30, 2025  
**App Name:** Self Audit Expense Tracker  
**Package Name:** `com.whattheapp.selfauditexpensetracker`  
**Developer Contact:** hakim.dilawar@gmail.com  

---

## 1. Overview & Core Privacy Commitment

**Self Audit Expense Tracker** is designed with a **privacy-first architecture**. 

We believe that your personal financial data belongs solely to you. All SMS and RCS message reading, message parsing, transaction categorization, and expense calculations take place **100% locally on your Android device**. 

- **No Data Uploads:** Your financial data, messages, and transaction history are never transmitted off your device.
- **No Cloud Storage:** We do not operate cloud servers to receive, store, or process your personal data.
- **No Remote Analytics or Tracking:** We do not use third-party analytics SDKs, tracking tools, or advertising networks.

---

## 2. Information Collection and Usage

Because all processing is performed strictly on-device, **we do not collect, store, or transmit any personal data to any external server.**

### Information Processed Locally:
- **SMS & RCS Messages:** Financial transaction alert messages sent by your banks, financial institutions, or payment providers.
- **Notifications:** Incoming bank and payment app notifications detected via Android's Notification Listener Service.
- **Expense Records:** Parsed transaction details including amount, merchant/vendor name, transaction date, and account category.

All of this data remains strictly inside the app's local private database on your device (`Room` database).

---

## 3. Detailed Explanation of Android Permissions

To provide automatic transaction detection and local expense auditing, Self Audit Expense Tracker requests specific Android permissions. Each permission is used exclusively for local processing:

| Permission | Purpose & Scope |
| :--- | :--- |
| `android.permission.READ_SMS` | Allows the app to scan SMS inbox locally to identify past financial transactions (debit/credit alerts from banks) and convert them into expense entries. |
| `android.permission.RECEIVE_SMS` | Allows the app to listen for incoming financial SMS messages in real-time to automatically log new expenses as they occur. |
| `android.permission.POST_NOTIFICATIONS` | Allows the app to display local status notifications (e.g., instant transaction detection alerts, daily budget summaries). |
| `android.permission.BIND_NOTIFICATION_LISTENER_SERVICE` (`NotificationListenerService`) | Allows the app to detect incoming financial app notifications and RCS transaction alerts locally. This enables transaction logging for banking apps, digital wallets, and messaging apps without relying solely on SMS. |

> **Important:** None of the data accessed through these permissions is ever uploaded, shared, or transmitted off your device.

---

## 4. Zero Third-Party Sharing & Data Selling

We adhere to a strict **Zero Data Sharing** policy:
- **No Cloud Servers:** We do not own, rent, or send data to any remote server or cloud service.
- **No Data Selling:** We do not sell, rent, trade, or monetize your personal or financial data under any circumstances.
- **No Third-Party SDKs:** The app contains no third-party ad networks, telemetry tools, or user behavior tracking libraries.

---

## 5. Data Security & Storage

- **Local Storage:** All application data, including custom categories, budgets, and transaction history, is stored securely within your device's isolated local application storage.
- **Data Retention & Control:** Your data stays on your device for as long as you keep the app installed. You can delete individual transaction records or wipe all app data at any time via the app settings or Android App Info screen.
- **App Uninstall:** Uninstalling the app permanently removes all locally stored app data from your device.

---

## 6. Children's Privacy

Self Audit Expense Tracker is not directed to children under the age of 13. We do not knowingly collect or request any personal information from children. Since all operations are 100% on-device, no information is collected from any user.

---

## 7. Changes to This Privacy Policy

We may update our Privacy Policy from time to time to reflect updates to the app or legal requirements. Any changes will be published in this repository with an updated "Effective Date".

---

## 8. Contact Information

If you have any questions, concerns, or feedback regarding this Privacy Policy or the app's privacy practices, please contact us at:

- **Email:** hakim.dilawar@gmail.com  
- **Developer:** Self Audit Expense Tracker Team  
- **Package Name:** `com.whattheapp.selfauditexpensetracker`

---

© 2026 Self Audit Expense Tracker. All rights reserved.
