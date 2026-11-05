# 📚 OpenShelf – Library Management System

OpenShelf is a full-stack web-based Library Management System designed to simplify traditional library operations and enhance the overall reading experience. It provides a centralized platform where users can discover books, request and reserve copies, manage borrowing activities, and interact with other readers.

The system also provides an administrative dashboard to manage books, users, borrowing requests, issuing, returns, and library activities efficiently.

## ✨ Features

### 👤 User Features

- **User Authentication:** Secure registration and login.
- **Book Discovery:** Browse, explore, and search for books.
- **Book Details:** View book information, availability, ratings, and reviews.
- **Book Requests:** Request books online.
- **Book Reservations:** Reserve books when copies become available.
- **Waitlist Management:** Join waitlists for unavailable books.
- **Borrowing Dashboard:** Track borrowed books and due dates.
- **Due-Date Reminders:** Receive reminders for upcoming and overdue returns.
- **Fine Management:** Automatic calculation of overdue fines.
- **Ratings and Reviews:** Rate books and share reading experiences.
- **Open Discussion:** Interact with other readers through discussions.
- **Words Worth Keeping:** Explore and save meaningful quotes.

### 🛠️ Admin Features

- **Admin Dashboard:** Monitor library activities.
- **Book Management:** Add, update, and manage books.
- **User Management:** View and manage registered users.
- **Request Management:** View and process book requests.
- **QR Code Generation:** Generate a unique QR code for each valid book request.
- **QR Code Scanning:** Scan QR codes through a camera or upload an image from the gallery.
- **QR Code Verification:** Validate the QR token and corresponding book request before issuing.
- **Direct Book Issuing:** Issue books directly after successful QR verification.
- **Borrowing Management:** Manage book issuing and returning records.
- **Fine Management:** Monitor overdue books and applicable fines.
- **Review Management:** Monitor and moderate user ratings and reviews.
- **Library Insights:** View top-rated and most-borrowed books.

## 📱 QR Code Generation & Redemption Workflow

OpenShelf implements a QR-based book issuing system to make the borrowing process faster and more efficient.

### How QR Code Generation Works

1. A user submits a book request.
2. The backend validates the request.
3. A unique token is generated for the valid request.
4. A QR code is created using the token.
5. The QR code is displayed to the user for administrative verification.

### How to Redeem a QR Code (Book Issuing)

1. The user visits the library with their generated QR code.
2. The administrator opens the QR scanner from the admin dashboard.
3. The administrator scans the QR code using the camera or uploads the QR image from the gallery.
4. The backend receives the QR token and verifies its authenticity.
5. The system checks whether the associated request is valid and eligible for issuing.
6. If verification succeeds, the administrator can issue the requested book.
7. The borrowing record is created and the book inventory is updated.
8. The QR request is marked as processed so that the same request cannot be redeemed again.

**QR Code Workflow:**

`Book Request → Unique Token Generation → QR Code Creation → Admin Scanning → Token Verification → Book Issuing → Request Processed`

## ⚙️ How OpenShelf Works

1. Users register or log in to the application.
2. They browse and search for books.
3. Users submit borrowing or reservation requests.
4. Administrators process valid requests using the QR code issuing system.
5. The system maintains borrowing and return records.
6. Automated background jobs check due dates and manage reminders.
7. Overdue fines are calculated according to configured library rules.
8. Readers can share reviews, ratings, quotes, and discussions.

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| React.js | Frontend development |
| TypeScript | Type safety |
| Bootstrap | Responsive UI |
| Node.js | Backend runtime |
| Express.js | REST API development |
| MongoDB | Database |
| MongoDB Atlas | Cloud database hosting |

## 🗄️ Database Management

MongoDB is used to store and manage application data.

Main data collections include:

- Users
- Books
- Borrows
- BookRequests
- Reviews
- Discussions

## 🚀 Getting Started

### Prerequisites

- Node.js
- npm
- MongoDB Atlas account
- Git

### Installation

**1. Clone the repository**

```bash
git clone https://github.com/tishaaamali/OpenShelf.git
```

**2. Navigate to the project folder**

```bash
cd OpenShelf
```

**3. Install dependencies**

Install dependencies separately inside the frontend and backend directories.

```bash
npm install
```

**4. Configure environment variables**

Create the required `.env` files and configure MongoDB connection details and other application settings.

Never upload private credentials or `.env` files to GitHub.

**5. Run the application**

Start the backend and frontend using their respective development scripts.

## 🎯 Project Objective

The primary objective of OpenShelf is to digitize traditional library operations, reduce manual work, improve book accessibility, and create an interactive reading community.

By combining library management features with QR-based book issuing, automated reminders, reservation management, and reader engagement features, OpenShelf provides a modern library management experience.

## 👩‍💻 Developer

**Tisha Mali**

Full-Stack Web Development Project

GitHub: [@tishaaamali](https://github.com/tishaaamali)

---

⭐ If you find this project interesting, consider giving the repository a star!
