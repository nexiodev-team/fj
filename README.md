# Nexio.dev | Faizan Jiffry Portfolio

This project is a specialized, high-quality online platform designed to establish the professional digital presence of **Mr. [cite_start]Faizan Jiffry**[cite: 58, 59, 91]. [cite_start]It serves as a centralized hub for educational resources, commerce subject expertise, and direct professional engagement[cite: 91, 153].

## 🎯 Project Objectives
* **Establish Expert Authority:** Showcase curriculum knowledge and student testimonials to build immediate trust.
* **Centralize Educational Resources:** Provide an intuitive platform to organize subject guides and teaching methodologies.
* **Enable Direct Engagement:** Incorporate accessible contact points for students and institutions.
* **Enhance Online Recognition:** Position Mr. Jiffry as a visible and available expert in the education sector.

---<img width="2605" height="1465" alt="ui" src="https://github.com/user-attachments/assets/8ba5135a-b009-436e-b7d4-e6bd67e82b36" />


## 🛠 Technology Stack
* **Framework:** Next.js + React.
* **Styling:** Tailwind CSS (Utility classes only).
* **Architecture:** Next.js `app/` directory for routing.

---

## 📂 Site Structure & Architecture
[cite_start]The project follows a modular structure where the `app/` folder handles routing and the `components/` folder houses reusable UI[cite: 15, 16].

**Sitemap:**
* **Home:** Main landing page.
* **About Me:** Professional background and teaching philosophy.
* **Class Schedule:** Details on recurring tuition sessions.
* **Seminars & Seminar Details:** Information on special educational events.
* **Past Papers:** A repository for student resources.
* **Contacts:** Direct inquiry tools for tuition and consulting.

---

## 🎨 Design Specifications
The implementation must match the approved visual identity and be fully responsive.

### Color Palette 
| Purpose | Color Name | Hex Code | Colors |
| :--- | :--- | :--- | :--- |
| Primary Accent | **Bright Red** | `#e30220` | ![](https://placehold.co/100x15/e30220/FFF) |
| Secondary Accent | **Deep Red** | `#bf0000`  | ![](https://placehold.co/100x15/bf0000/FFF) |
| Primary Text/BG | **Near Black** | `#242024`  | ![](https://placehold.co/100x15/242024/FFF) |
| Secondary BG | **Light Grey** | `#dddddd`  | ![](https://placehold.co/100x15/dddddd/FFF) |
| Neutral | **Off White** | `#f3f4f5`  | ![](https://placehold.co/100x15/f3f4f5/FFF) |

---

# Local Development Guide

Before you begin, ensure that the following tools are installed on your system:

- **Node.js** (LTS version recommended)
- **npm** (comes bundled with Node.js) or **yarn**
- **Git**

Verify the installations by running:
```bash
node -v
npm -v
git --version 
```

#### 1. Clone the Repository and navigate to the project directory
```bash
git clone <repository-url>
cd <project-folder-name>
```

#### 2. Then install dependencies 
Using npm
```bash
npm install
```
Using yarn
```bash
yarn install
```
This will install all dependencies listed in the `package.json` file. 

#### 3. Run the Development Server
Using npm
```bash
npm run dev
```
Using yarn
```bash
yarn dev
```

#### 4. Access the Application
Once the development server is running, open your browser and navigate to:
```bash
[yarn dev](http://localhost:3000)
```
The application will automatically reload when changes are made to the source code.

#### 5. Stopping the Server
To stop the development server, press: `Ctrl + C`

# File Structure

```
my-app/
├── public/                 # Static assets (images, fonts, etc.)
├── src/                    # All source code (best practice to keep root clean)
│   ├── app/                # NEXT.JS APP ROUTER (Routing Layer only)
│   │   ├── (auth)/         # Route Group: Logical grouping for clean URLs
│   │   │   ├── login/
│   │   │   │   └── page.tsx
│   │   │   └── layout.tsx
│   │   ├── (dashboard)/
│   │   │   ├── settings/
│   │   │   └── page.tsx
│   │   ├── api/            # API Route Handlers
│   │   ├── layout.tsx      # Root Layout (Providers live here)
│   │   └── page.tsx        # Homepage
│   ├── components/         # SHARED UI COMPONENTS
│   │   ├── ui/             # Shadcn/Radix-style primitives (Button, Input)
│   │   ├── forms/          # Reusable form wrappers
│   │   └── layout/         # Shared Shells (Navbar, Sidebar, Footer)
│   ├── features/           # FEATURE-DRIVEN MODULES (Domain Logic)
│   │   ├── user-profile/   # Everything specific to "User Profile"
│   │   │   ├── components/ # Local components only used in this feature
│   │   │   ├── hooks/      # Local hooks (e.g., useProfileData)
│   │   │   ├── services/   # Data fetching/API calls for this feature
│   │   │   ├── types.ts    # Type definitions for this feature
│   │   │   └── index.ts    # Public API: Export only what other features need
│   │   └── billing/        # Another feature module
│   ├── hooks/              # Global reusable hooks
│   ├── lib/                # Third-party configurations (Prisma, Stripe, Supabase)
│   ├── services/           # Global services (Analytics, Logger, Mail)
│   ├── store/              # State management (Zustand/Redux)
│   ├── types/              # Global TypeScript types
│   └── utils/              # Pure helper functions (date formatting, etc.)
├── .env.local              # Secrets
├── next.config.ts          # Next.js Config
└── tsconfig.json           # Path aliases (@/*)
```
