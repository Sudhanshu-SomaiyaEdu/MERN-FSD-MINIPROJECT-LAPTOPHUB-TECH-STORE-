# 🛍️ Tech Store (Laptop Hub)

**Tech Store (Laptop Hub)** is a modern full-stack e-commerce web application built for showcasing and selling premium laptops and accessories.  
It offers a **sleek UI**, **secure checkout**, and **seamless product browsing experience**, designed using **React, TypeScript, TailwindCSS, and PostgreSQL**.

---

## 🚀 Tech Stack

| Layer | Technologies |
|--------|---------------|
| **Frontend** | React, TypeScript, Vite, TailwindCSS, ShadCN/UI, Framer Motion |
| **Backend** | Express.js, PostgreSQL (via Drizzle ORM), Stripe (Payments), Passport.js |
| **Database** | PostgreSQL |
| **Build Tools** | Vite, Esbuild, PostCSS, Autoprefixer |
| **Dev Tools** | TypeScript, Replit Dev Plugins, ESLint |

---

## 📂 Project Structure

```
Tech Store (Laptop Hub)
├── client/
│   ├── src/
│   ├── index.html
│   └── tailwind.config.ts
├── server/
│   ├── index.ts
│   └── routes/
├── shared/
│   └── schema.ts
├── drizzle.config.ts
├── postcss.config.js
├── tsconfig.json
├── vite.config.ts
├── package.json
├── components.json
├── design_guidelines.md
└── .gitignore
```

---

## ⚙️ Setup Instructions

### 🧩 1. Clone the Repository
```bash
git clone https://github.com/yourusername/tech-store-laptop-hub.git
cd tech-store-laptop-hub
```

### 📦 2. Install Dependencies
```bash
npm install
```

### 🔑 3. Configure Environment Variables
Create a `.env` file in the root directory:
```env
DATABASE_URL=postgresql://user:password@localhost:5432/laptophub
STRIPE_SECRET_KEY=your_stripe_secret
SESSION_SECRET=your_secret
```

### 🗃️ 4. Run Database Migration
```bash
npm run db:push
```

### ▶️ 5. Start the Application
```bash
npm run dev
```

---

## 🧠 Key Configuration Snapshots

### 🪄 Tailwind Configuration
```ts
// tailwind.config.ts
export default {
  darkMode: ["class"],
  content: ["./client/index.html", "./client/src/**/*.{js,jsx,ts,tsx}"],
  theme: {
    extend: {
      colors: {
        primary: { DEFAULT: "hsl(var(--primary))" },
        background: "hsl(var(--background))",
        foreground: "hsl(var(--foreground))"
      }
    }
  }
}
```

### ⚙️ PostCSS Setup
```js
// postcss.config.js
export default {
  plugins: {
    tailwindcss: {},
    autoprefixer: {},
  },
}
```

### 🧩 TypeScript Config
```json
{
  "include": ["client/src/**/*", "shared/**/*", "server/**/*"],
  "compilerOptions": {
    "strict": true,
    "module": "ESNext",
    "jsx": "preserve",
    "paths": {
      "@/*": ["./client/src/*"],
      "@shared/*": ["./shared/*"]
    }
  }
}
```

---

## 🖼️ Project Screenshots !

### 🏠 Homepage
![Homepage](./Screenshot%202025-11-08%20160729.png)

### 💻 Product Listing Page
![Product Listing](./Screenshot%202025-11-08%20160756.png)

### 🛒 Cart Page
![Cart Page](./Screenshot%202025-11-08%20160839.png)

### 📦 Checkout Page
![Checkout Page](./Screenshot%202025-11-08%20160903.png)

---

## 🎨 Design System

Refer to [`design_guidelines.md`](./design_guidelines.md) for:
- Typography hierarchy (Inter + Space Grotesk)
- Product grid spacing & card layout
- Navigation and button design
- Responsive container system

---

## ✨ Features

- 🔍 Product Search & Filters  
- 🛒 Add to Cart / Checkout Flow  
- 💰 Stripe Integration  
- 👤 Authentication System  
- 📊 Admin Dashboard (WIP)  
- 🌗 Dark Mode Ready  
- 📱 Fully Responsive UI  

---

## 🧱 Scripts

| Command | Description |
|----------|-------------|
| `npm run dev` | Start development server |
| `npm run build` | Build production files |
| `npm run start` | Run production server |
| `npm run db:push` | Apply Drizzle ORM migrations |

---

## 📸 Output Summary

| Page | Description |
|------|--------------|
| **Homepage** | Hero banner & CTA |
| **Products** | All laptop listings with filters |
| **Cart** | Checkout summary with item count |
| **Checkout** | Stripe-powered payment page |

---



---

## 👨‍💻 Author
**Sudhanshu Bramhraj**  and **Ayush Birari**  