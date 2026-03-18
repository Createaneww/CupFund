# ☕ CupFund – Support Your Favorite Creators

CupFund is a Patreon-inspired creator support platform that allows fans to contribute financially to creators through one-time or recurring payments.  
Built with **Next.js**, **Node.js**, and **MongoDB**, CupFund integrates **Razorpay** for secure and seamless payments.


## 📌 Table of Contents
- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Project Structure](#-project-structure)
- [Installation & Setup](#-installation--setup)
- [Usage](#-usage)
- [Future Enhancements](#-future-enhancements)
- [License](#-license)

---

## 🚀 Features

### 🔑 User Authentication
- Secure authentication system for **creators** and **supporters**.
- Role-based access using **JWT tokens**.
- Session handling with **NextAuth**.

### 👤 Creator Profiles
- Creators can create personalized profile pages with bio, avatar, and social links.
- Exclusive content for supporters who have contributed.

### 💳 Payment Integration (Razorpay)
- One-time and recurring payments via **Razorpay**.
- Secure checkout and transaction handling.
- Payment history stored in MongoDB.

### 📜 Content & Dashboard
- Creators can post content, updates, and messages for supporters.
- Dashboard with **earnings overview**, supporter count, and latest transactions.

### 📱 Responsive UI
- Fully responsive with **Tailwind CSS**.
- Optimized for mobile, tablet, and desktop devices.

---

## 🛠 Tech Stack

**Frontend:**
- [Next.js](https://nextjs.org/) – React-based framework with server-side rendering.
- Tailwind CSS – Modern utility-first CSS framework.

**Backend:**
- [Node.js](https://nodejs.org/) – JavaScript runtime for backend logic.
- [Express.js](https://expressjs.com/) – Web framework for APIs.

**Database:**
- [MongoDB](https://www.mongodb.com/) – NoSQL database for storing users, payments, and content.

**Payments:**
- [Razorpay](https://razorpay.com/) – Payment gateway integration.

**Authentication:**
- [NextAuth](https://next-auth.js.org/) + JWT – Secure authentication.

---

## 📂 Project Structure

```
CupFund/
│
├── my-app/                      # Main project directory
│   ├── app/                      # Next.js App Router pages
│   │   ├── api/                  # API routes for auth & payments
│   │   ├── dashboard/            # Dashboard page
│   │   ├── login/                 # Login page
│   │   ├── about/                 # About page
│   │   └── [username]/            # Dynamic creator profiles
│   │
│   ├── componets/                # Reusable UI components
│   │   ├── Dashboard.js
│   │   ├── Navbar.js
│   │   ├── Footer.js
│   │   └── PaymentPage.js
│   │
│   ├── models/                   # Mongoose models
│   │   ├── User.js
│   │   └── Payment.js
│   │
│   ├── db/                       # MongoDB connection
│   │   └── connectDb.js
│   │
│   ├── public/                   # Static assets
│   ├── globals.css               # Global styles
│   ├── package.json
│   └── next.config.mjs
│
└── README.md
```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the repository
```bash
git clone https://github.com/yourusername/CupFund.git
cd CupFund-main/my-app
```

### 2️⃣ Install dependencies
```bash
npm install
```

### 3️⃣ Set up environment variables  
Create a `.env.local` file in `/my-app`:
```
MONGO_URI=your_mongodb_connection_string
RAZORPAY_KEY_ID=your_razorpay_key_id
RAZORPAY_KEY_SECRET=your_razorpay_secret
NEXTAUTH_SECRET=your_nextauth_secret
NEXTAUTH_URL=http://localhost:3000
```

### 4️⃣ Start the development server
```bash
npm run dev
```

App will be live at:  
```
http://localhost:3000
```

---

## 🎯 Usage

1. **Sign Up / Login** as a creator or supporter.
2. Creators can set up their profile and share exclusive content.
3. Supporters can browse creator pages and make payments via Razorpay.
4. View payment history and dashboard analytics.

---

## 🔮 Future Enhancements
- Multiple payment gateways (Stripe, PayPal).
- Creator tiers with different perks.
- Email notifications for payments.
- Advanced analytics dashboard.

---

## 📜 License
This project is licensed under the **MIT License**.

---

## 🤝 Contributing
Pull requests are welcome! For major changes, open an issue first to discuss your ideas.
