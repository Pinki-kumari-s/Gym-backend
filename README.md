# 🔧 Gym Website – Backend

This is the backend for the Gym Website developed using Node.js and Express. It handles sending emails via a contact form on the frontend and includes configuration for CORS and environment variables.

---

## 🛠️ Tech Stack

- Node.js
- Express.js
- Nodemailer
- dotenv
- CORS

---

## 📦 Setup Instructions

Follow the steps below to run the backend server locally:

1. **Clone the repository**

```bash
git clone https://github.com/Pinki-Kumari-s/Gym-backend.git
cd Gym-backend
```

2. **Install dependencies**

```bash
npm install
```

3. **Create `.env` file**

Create a `.env` file in the root folder and add the following:

```env
PORT=5000
FRONTEND_URL=http://localhost:5173
SMTP_HOST=smtp.gmail.com
SMTP_PORT=587
SMTP_USER=your_email@example.com
SMTP_PASS=your_app_password
```

> ⚠️ If you're using Gmail, make sure to enable [2-Step Verification](https://myaccount.google.com/security) and generate an [App Password](https://support.google.com/accounts/answer/185833?hl=en) for secure email sending.

4. **Start the server**

```bash
node index.js
```

The server will run on: `http://localhost:5000`

---

## 📁 Folder Structure

```
gym-backend/
├── utils/
│   └── sendEmail.js
├── index.js
├── .env
├── package.json
└── README.md
```

---

## 🔐 API Endpoint

### POST `/api/contact`

**Request Body:**
```json
{
  "name": "John Doe",
  "email": "john@example.com",
  "message": "I want to join your gym"
}
```

**Function:** Sends an email using the SMTP credentials to your inbox.

---

## 🚀 Features

- ✅ Sends email from frontend form
- 🌍 CORS enabled for cross-origin frontend access
- 📦 Lightweight & fast backend
- 🔐 Secure with environment variables

---

## 🧠 Tip for Production

- Use a service like **Render**, **Railway**, or **Vercel Functions** to deploy.
- Add `.env` variables securely in the deployment dashboard.

---

## 📩 Contact

For support or questions, contact [sanjayyadavmintadevi@gmail.com](mailto:sanjayyadavmintadevi@gmail.com.com
