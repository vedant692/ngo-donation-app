# Donation Management Platform

A web-based application designed to streamline donation collection and management. This platform allows users to register, donate via PayPal, and track their transaction status, while providing Admins and Super Admins with powerful tools to oversee funds and manage user roles.

## 🚀 Key Features

### User Panel
* **Secure Authentication:** User Login and Registration.
* **Donation Processing:** Seamless redirection to PayPal for payments.
* **Transaction Verification:** Payments are verified via Transaction ID.
* **Payment History:** Users can view all past donations and their real-time status (Pending, Done, Failed).

### Admin Panel
* **Dashboard:** View total funds gathered and total donor count.
* **Detailed Reporting:** Monitor payments per person with status indicators.
* **Status Management:** Track Pending, Completed, and Failed transactions.

### Super Admin (RBAC)
* **Exclusive Access:** Only one Super Admin exists.
* **Role Management:** Ability to create new Admins, remove Admins, or demote them to normal users.

## ⚠️ Important Configuration & Security

**1. Super Admin Setup (Crucial)**
The Super Admin credentials are currently initialized in the backend for convenience.
* **Action Required:** Upon cloning, navigate to the backend configuration and **immediately update/remove** the hardcoded Super Admin credentials before deploying to production.

**2. Payment Gateway**
The project is set up to redirect to PayPal.
* Update the PayPal client ID/Secret in your environment variables to link your specific donation account.

## 🛠️ Tech Stack
* **Frontend:** React.js, HTML, CSS
* **Backend:** Node.js
* **Database:** MongoDB

## 📦 Installation

1.  Clone the repository:
    ```bash
    git clone [https://github.com/vedant692/ngo-donation-app](https://github.com/vedant692/ngo-donation-app)
    ```
2.  Navigate to the project directory and install dependencies:
    ```bash
    npm install
    ```
    *(Note: You may need to install dependencies for both client and server folders if separated).*

3.  Set up your environment variables (e.g., Database URI, PayPal Keys).
4.  Run the application:
    ```bash
    npm start
    ```

## 🤝 Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## 📄 License
[MIT](https://choosealicense.com/licenses/mit/)
