# OmniDine System

**OmniDine** is a full-stack restaurant chain management system built with Node.js and PostgreSQL. It provides functionality for managing customers, menu items, transactions, and multiple franchise locations—all through a web interface. Designed for scalable operations with support for loyalty memberships, multiple payment types, and franchise analytics.

---

## 🧠 Key Features

- Customer account creation and loyalty tracking
- Diverse menu items (Asian cuisine emphasis)
- Order placement and payment (cash or card)
- Tax and tip calculation
- Multi-location franchise tracking
- Transaction and revenue dashboards

---

## 🗂️ Project Structure

```
omnidine-system/
│
├── index.js              # Main server entry point
├── package.json
├── .env                  # Local environment variables (not committed)
│
├── routes/               # Express route handlers
│   ├── customerRoutes.js
│   ├── menuRoutes.js
│   └── franchiseRoutes.js
│
├── views/                # HTML pages rendered to users
│   ├── homepage.html
│   ├── customers.html
│   ├── dashboard.html
│   ├── franchises.html
│   ├── add-customer.html
│   ├── menu-items.html
│   ├── place-order.html
│   └── transactions.html
│
├── public/               # (Optional) static assets like CSS/JS/images
│
├── sql/                  # SQL schema and data scripts
│   ├── Restaurant_V18.sql
│   ├── output_file.sql
│   ├── output v2.sql
│   └── output3.sql
│
├── controllers/ (optional) # Logic separation (if used)
│   ├── customers.js
│   └── place-orders.js
│
├── Description.pdf
├── README.md
```

---

## ⚙️ Technologies Used

- **Node.js + Express**
- **PostgreSQL**
- **HTML5 / CSS3 / JS**
- Environment variables via `dotenv`

---

## 🚀 Getting Started

### 1. Install Dependencies

```bash
npm install
```

### 2. Create the PostgreSQL Database

```bash
createdb Restaurant
psql Restaurant < sql/Restaurant_V18.sql
```

You can also copy the contents of `Restaurant_V18.sql` into your PostgreSQL Query Tool and run it manually.

### 3. Configure `.env`

Create a `.env` file in the root directory with the following structure:

```
DATABASE_URL=postgresql://<your_username>:<your_password>@localhost:5432/Restaurant
PORT=3000
```

Replace `<your_username>` and `<your_password>` with your local PostgreSQL credentials.

### 4. Start the Server

```bash
node index.js
```

Then open your browser to:

```
http://localhost:3000
```

---

## 🧩 App Modules

| Feature | Description |
|--------|-------------|
| **Homepage** | Navigation landing page |
| **Customer Management** | View, add, and update customers and memberships |
| **Menu Display** | Browse food & beverage options |
| **Place Order** | Submit food orders with payment details |
| **Transactions** | Track past orders and tips |
| **Dashboard** | Basic analytics overview |
| **Franchise Locations** | List of restaurant locations |

---

## 🧪 Notes for Reviewers

Thank you for reviewing **OmniDine**. If you experience any setup issues, please feel free to reach out via Discord or email.

This project demonstrates core concepts in:

- Relational database design
- Web server routing with Node.js
- Real-world schema implementation for a multi-unit business
- Full CRUD functionality with a user-friendly interface

Happy grading!

— Team Cann-E
