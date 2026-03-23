# 🍽️ Campus Canteen – Food Ordering System

A web-based canteen management and food ordering system built for college campuses. Students can browse the menu, place orders, and track them in real time, while admins manage the full menu and order pipeline from a dedicated dashboard.

---

## 📌 Table of Contents

- [About the Project](#about-the-project)
- [Pages & Features](#pages--features)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Admin Credentials (Demo)](#admin-credentials-demo)
- [Known Limitations](#known-limitations)
- [Future Improvements](#future-improvements)
- [Contributing](#contributing)
- [License](#license)

---

## About the Project

Campus Canteen is a front-end-only web application that simulates a complete canteen ordering system. It allows students to register, log in, browse food categories, add items to a cart, place orders, and track delivery status. Admins get a separate protected panel to manage menu items and view orders.

All data is stored in the browser's `localStorage` — no backend or database is required to run this project.

---

## Pages & Features

| Page | File | Description |
|---|---|---|
| 🏠 Homepage | `Homepage.html` | Landing page with hero section, features overview, and dark/light mode toggle |
| 📋 Menu | `Newmenue1.html` | Browse food items by category, add to cart, view cart |
| 👤 Register / Login | `Registrationpage.html` | User sign-up and login with email/password; Google & Facebook OAuth buttons (UI only) |
| 🙍 User Profile | `userprofile.html` | View and manage logged-in user's profile and order history |
| 📦 Order Tracking | `Ordertracking1.html` | Track current order status with a step-by-step progress indicator and feedback form |
| ℹ️ About Us | `about-us.html` | Information about the canteen, team, and mission |
| 🔐 Admin Login | `Admin_login.html` | Secure login page for canteen administrators |
| ⚙️ Admin Dashboard | `Admin1.html` | Add/edit/delete menu items, manage categories, view and update order statuses |

### Highlighted Features

- 🌙 Dark / Light mode toggle across all pages
- 🛒 Shopping cart with item quantity management
- 🔐 Role-based access — separate flows for students and admins
- 📱 Responsive design — works on mobile and desktop
- 📦 Real-time order tracking UI with status steps
- ⭐ Order feedback / rating form
- 💾 Fully localStorage-based (no server needed)

---

## Tech Stack

| Technology | Usage |
|---|---|
| HTML5 | Page structure and layout |
| CSS3 | Styling, animations, dark/light mode via CSS variables |
| Vanilla JavaScript | All interactivity, form handling, localStorage logic |
| [Font Awesome 6](https://fontawesome.com/) | Icons throughout the UI |
| [Google Fonts](https://fonts.google.com/) | Montserrat and Playfair Display fonts |
| localStorage | Persisting users, menu items, and orders in the browser |

---

## Project Structure

```
campus-canteen/
│
├── Homepage.html            # Landing / Home page
├── Newmenue1.html           # Food menu & cart
├── Registrationpage.html    # User login & registration
├── userprofile.html         # User profile page
├── Ordertracking1.html      # Order tracking page
├── about-us.html            # About us page
├── Admin_login.html         # Admin login
└── Admin1.html              # Admin dashboard
```

> ℹ️ All pages are self-contained HTML files. There is no build step or package manager required.

---

## Getting Started

Since this is a plain HTML project, you do **not** need Node.js, npm, or any server.

### Option 1 — Open directly in browser

1. Download or clone this repository:
   ```bash
   git clone https://github.com/your-username/campus-canteen.git
   ```
2. Open `Homepage.html` in any modern web browser (Chrome, Firefox, Edge).

### Option 2 — Use Live Server (recommended for development)

If you use **VS Code**, install the [Live Server extension](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer), right-click `Homepage.html`, and select **"Open with Live Server"**. This avoids any browser CORS issues when navigating between pages.

---

## Admin Credentials (Demo)

The admin panel uses hardcoded demo credentials stored in `localStorage` on first load.

| Field | Value |
|---|---|
| Username | `admin` |
| Password | `password123` |

> ⚠️ These are **demo credentials only**. Do not use this authentication method in a production environment.

---

## Known Limitations

- **No real backend** — all data lives in `localStorage` and is lost if the browser cache is cleared.
- **No real authentication** — passwords are stored as plain text in `localStorage`. This is not secure and should never be used in production.
- **Google / Facebook OAuth** — the social login buttons are UI placeholders. A real Client ID and OAuth flow must be configured to make them functional.
- **No payment gateway** — the ordering flow is simulated; no real transactions occur.
- **Single-device only** — because data is in `localStorage`, orders placed on one device are not visible on another.

---

## Future Improvements

- [ ] Connect to a real backend (Node.js + Express or Firebase)
- [ ] Use a database (MongoDB, PostgreSQL, or Firestore) for persistent data
- [ ] Implement real JWT-based authentication
- [ ] Integrate a payment gateway (Razorpay, Stripe)
- [ ] Add push notifications for order status updates
- [ ] Build a mobile app version (React Native / Flutter)

---

## Contributing

Contributions are welcome! To contribute:

1. Fork this repository
2. Create a new branch: `git checkout -b feature/your-feature-name`
3. Make your changes and commit: `git commit -m "Add your feature"`
4. Push to your fork: `git push origin feature/your-feature-name`
5. Open a Pull Request

---

## License

This project is open source and available under the [MIT License](LICENSE).

---

> Made with ❤️ for campus life
