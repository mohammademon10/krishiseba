# 🌾 KrishiSheba Frontend

A modern, responsive, and accessible frontend interface for the **KrishiSheba** platform – connecting farmers and agricultural equipment providers across Bangladesh.

Built with **HTML5**, **CSS3**, and **Vanilla JavaScript**, this frontend interfaces seamlessly with the Spring Boot backend.




## ✨ Overview

KrishiSheba empowers the agricultural sector with a user-friendly, secure web platform:

- 👨‍🌾 **Farmers** can browse and rent farming equipment.
- 🛠️ **Retailers** can list and manage their inventory.
- 🛡️ **Admins** can oversee platform operations and approve listings.

This frontend delivers a clean, mobile-first experience with progressive enhancement and accessibility in mind.



## 🖥️ Tech Stack

- **HTML5** – semantic structure
- **CSS3** – responsive layout and modern UI
- **JavaScript (ES6)** – interactive features, API integration
- **Bootstrap Icons** – for clean visuals
- **Inter Font** – optimized typography
- Backend integration: via REST API (Spring Boot)





## 📂 Project Structure
krishisheba-frontend/
├── index.html # Landing page
├── login.html # Login form for all roles
├── register.html # Registration form
├── farmerDashboard.html # Farmer interface
├── retailerDashboard.html # Retailer interface
├── adminDashboard.html # Admin interface
├── assets/
│ ├── css/
│ │ └── style.css # Global styles
│ ├── js/
│ │ └── app.js # Core JS logic and API handling
│ └── images/ # Static images and icons
└── README.md




## 🎨 UI/UX Features

- 📱 **Mobile-first** responsive layout
- 🎨 **Modern design system** with subtle animations
- ♿ **Accessibility** compliant (WCAG 2.1 AA)
- 💡 **Dark/light mode ready** (optional future support)
- 🔍 **Searchable equipment catalog** with filters
- 🔒 **Role-based UI rendering** (Farmer, Retailer, Admin)





## 🔐 Security & Best Practices

- All API calls made via **HTTPS**
- JWT stored in **memory/sessionStorage** (never localStorage)
- Form inputs validated on client-side
- Rate-limiting and CSRF handled via backend
- Sanitized DOM manipulation to avoid XSS





## 🚀 Getting Started

### 📦 Prerequisites

- A simple local server (like Live Server in VS Code)
- Backend API running on `http://localhost:8080`



### 🔧 Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-org/krishisheba-frontend.git
   cd krishisheba-frontend
Open index.html with Live Server
Or launch with:

bash
Copy
Edit
npx serve .
Ensure backend API is running (for login, equipment, etc.)

🔗 API Integration
JavaScript (app.js) handles REST API calls:

POST /api/auth/login – login

GET /api/equipment – get equipment list

POST /api/rentals – rent equipment

GET /api/admin/users – admin user management

Tokens are included in Authorization headers as Bearer <token>.



| Page                     | Description                     | Access        |
| ------------------------ | ------------------------------- | ------------- |
| `index.html`             | Landing & intro                 | Public        |
| `login.html`             | Login (Farmer, Retailer, Admin) | Public        |
| `register.html`          | User registration               | Public        |
| `farmerDashboard.html`   | Browse equipment, rent, profile | Farmer only   |
| `retailerDashboard.html` | Manage listings, requests       | Retailer only |
| `adminDashboard.html`    | Approve equipment, manage users | Admin only    |



📈 Features Under Development
🔔 Notification system for rental status

🌐 Multi-language support (Bangla/English)

💳 Payment gateway integration

📦 Offline-first PWA capabilities

🔄 Real-time data refresh (WebSockets)



🧪 Testing & Debugging

While no testing framework is used here:

✅ Manual form validation checks

✅ API call simulations using Postman

✅ Browser dev tools for debugging

✅ Responsive layout tests via Chrome DevTools



🗺️ Roadmap

✅ Version 1.0
All main dashboard templates

Secure API integration

Role-based content

Search and filter equipment

Mobile-first UI

🔜 Version 1.1
React/Vue migration (optional)

Service worker caching

Payment system

SMS alert via Twilio API

🔮 Version 2.0
Full PWA support

Real-time notifications

Voice interface for farmers

AI-driven equipment suggestion



🙌 Contributing
Fork the repo

Create a new branch:
git checkout -b feature/awesome-feature

Make changes and commit:
git commit -m "Add awesome feature"

Push the changes:
git push origin feature/awesome-feature

Open a pull request

Guidelines
Use semantic HTML

Keep styles modular and reusable

Write clean, commented JS

Keep UI consistent with backend design


📝 License
This project is licensed under the MIT License. See the LICENSE file for details.



📞 Support
📘 Docs: Coming soon

🐛 Report Issues: GitHub Issues

✉️ Email: support@krishisheba.com



💚 Made with love for the farmers of Bangladesh 🇧🇩
