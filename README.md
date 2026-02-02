# 🚀 Job & Networking Portal

<div align="center">

![Job Portal](https://img.shields.io/badge/Job_Portal-v1.0.0-blue)
![React](https://img.shields.io/badge/React-18.3.1-61DAFB?logo=react)
![Node.js](https://img.shields.io/badge/Node.js-Express-339933?logo=node.js)
![MongoDB](https://img.shields.io/badge/MongoDB-Atlas-47A248?logo=mongodb)
![Clerk](https://img.shields.io/badge/Auth-Clerk-6C47FF)

**A modern full-stack job portal platform inspired by LinkedIn, Upwork, and AngelList**

[Live Demo](https://job-portal-beta-bice.vercel.app) • [API Docs](#api-endpoints) • [Report Bug](https://github.com/yourusername/job-portal/issues)

</div>

---
<img width="1468" height="796" alt="image" src="https://github.com/user-attachments/assets/32bc3e7a-89bf-4695-85e8-3fa22e743d77" />
<img width="1470" height="797" alt="image" src="https://github.com/user-attachments/assets/01c20c55-373e-4f38-b7e7-a175b520d18c" />
<img width="1470" height="799" alt="image" src="https://github.com/user-attachments/assets/4e2e389c-ad76-4daa-8b57-a6069745ae9b" />
<img width="1470" height="806" alt="image" src="https://github.com/user-attachments/assets/35b67939-a866-4a24-a9eb-c1484535c657" />
<img width="1470" height="804" alt="image" src="https://github.com/user-attachments/assets/c10a50e2-9e22-49e0-bee9-d48730ede211" />
<img width="1467" height="795" alt="image" src="https://github.com/user-attachments/assets/c06f8ea1-4849-4513-994c-c190d3081b21" />
<img width="1461" height="800" alt="image" src="https://github.com/user-attachments/assets/2b641ca6-3094-463f-aa74-5ac595312810" />
<img width="1468" height="797" alt="image" src="https://github.com/user-attachments/assets/a91513d6-7221-4c40-b3f7-b206c839d68d" />
<img width="1460" height="798" alt="image" src="https://github.com/user-attachments/assets/2897c62c-b2f9-4fcf-82a5-326d38df472e" />

## 📋 Table of Contents

- [Overview](#-overview)
- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Project Structure](#-project-structure)
- [Getting Started](#-getting-started)
- [Environment Variables](#-environment-variables)
- [API Documentation](#-api-documentation)
- [Deployment](#-deployment)
- [GTM Strategy](#-gtm-strategy)
- [Future Roadmap](#-future-roadmap)
- [Contributing](#-contributing)

---

## 🎯 Overview

The **Job & Networking Portal** is a comprehensive full-stack application designed to connect job seekers with companies. Built as part of the **RizeOS Core Team Internship Assessment**, this platform demonstrates proficiency in modern web development, authentication systems, cloud deployment, and product thinking.

### 🎥 Demo Video
**[📺 Watch 15-Minute Product Walkthrough](YOUR_DEMO_VIDEO_LINK)**

### 🌐 Live Deployments
- **Frontend (Vercel):** https://job-portal-beta-bice.vercel.app
- **Backend (Render):** https://job-portal-ordg.onrender.com

---

## ✨ Features

### 👤 User Features
- **🔐 Authentication & Authorization**
  - Secure user authentication via Clerk (OAuth, Email/Password)
  - JWT-based session management
  - Protected routes and role-based access control

- **📝 Profile Management**
  - Create and edit user profiles (name, bio, image)
  - Upload and manage resume (PDF support via Cloudinary)
  - View application history and status tracking

- **💼 Job Discovery**
  - Browse all active job listings with advanced filters
  - Search by title, location, salary, experience level
  - Real-time job availability updates
  - Detailed job descriptions with company information

- **📬 Job Applications**
  - One-click job application system
  - Track application status (Pending/Accepted/Rejected)
  - Download submitted resume
  - Prevent duplicate applications

### 🏢 Company/Recruiter Features
- **🔑 Company Registration & Login**
  - Separate authentication flow for companies
  - Company profile with logo upload (Cloudinary CDN)
  - Secure JWT token-based authorization

- **📋 Job Management Dashboard**
  - Post new job openings with rich descriptions
  - Edit and delete job postings
  - Toggle job visibility (active/inactive)
  - Track total applicants per job

- **👥 Applicant Management**
  - View all applications for posted jobs
  - Filter applicants by job, status, or date
  - Change application status (Accept/Reject)
  - Download candidate resumes
  - Detailed applicant profiles

### 🎨 UI/UX Highlights
- **Responsive Design** - Fully mobile-optimized using Tailwind CSS
- **Modern Aesthetics** - Clean, professional interface with smooth animations
- **Intuitive Navigation** - Context-aware navigation and breadcrumbs
- **Loading States** - Custom loaders for better user experience
- **Toast Notifications** - Real-time feedback for all actions
- **Dark Mode Ready** - Prepared for theme switching

---

## 🛠 Tech Stack

### Frontend
| Technology | Purpose |
|------------|---------|
| **React 18.3.1** | Component-based UI library |
| **Vite** | Lightning-fast build tool |
| **Tailwind CSS** | Utility-first CSS framework |
| **Clerk React** | Authentication & user management |
| **Axios** | HTTP client for API requests |
| **React Router DOM** | Client-side routing |
| **React Toastify** | Toast notifications |
| **Lucide React** | Modern icon library |
| **Quill.js** | Rich text editor for job descriptions |
| **Moment.js** | Date formatting and manipulation |

### Backend
| Technology | Purpose |
|------------|---------|
| **Node.js + Express** | Server runtime & web framework |
| **MongoDB Atlas** | Cloud-hosted NoSQL database |
| **Mongoose** | MongoDB ODM with schema validation |
| **Clerk Express** | Backend authentication middleware |
| **JWT** | Stateless authentication tokens |
| **Bcrypt** | Password hashing |
| **Multer** | File upload handling |
| **Cloudinary** | Cloud-based image/file storage |
| **Sentry** | Error tracking and monitoring |
| **CORS** | Cross-Origin Resource Sharing |

### DevOps & Deployment
| Service | Purpose |
|---------|---------|
| **Vercel** | Frontend hosting with auto-deployment |
| **Render** | Backend hosting with auto-scaling |
| **MongoDB Atlas** | Managed database with backups |
| **Cloudinary CDN** | Global asset delivery network |
| **GitHub** | Version control and CI/CD |

---

## 📁 Project Structure

```
job-portal/
│
├── client/                          # Frontend React Application
│   ├── public/
│   │   ├── newFavicon.svg          # App favicon
│   │   └── vite.svg
│   │
│   ├── src/
│   │   ├── assets/                  # Static assets (images, icons, PDFs)
│   │   │   ├── logo.svg
│   │   │   ├── bg-image-main.jpg
│   │   │   ├── app_main_img.png
│   │   │   └── [50+ UI assets]
│   │   │
│   │   ├── components/              # Reusable React components
│   │   │   ├── Navbar.jsx          # Main navigation bar
│   │   │   ├── Footer.jsx          # Site footer
│   │   │   ├── Hero.jsx            # Landing page hero section
│   │   │   ├── JobListing.jsx      # Job cards grid display
│   │   │   ├── JobCard.jsx         # Individual job card
│   │   │   ├── RecruiterLogin.jsx  # Company login modal
│   │   │   ├── Calltoaction.jsx    # CTA section
│   │   │   ├── AppDownload.jsx     # Mobile app promo
│   │   │   └── Loading.jsx         # Loading spinner
│   │   │
│   │   ├── context/
│   │   │   └── AppContext.jsx      # Global state management (jobs, user, auth)
│   │   │
│   │   ├── pages/                   # Page-level components
│   │   │   ├── Home.jsx            # Landing page
│   │   │   ├── ApplyJob.jsx        # Job detail & application page
│   │   │   ├── Applications.jsx    # User's application history
│   │   │   ├── Dashboard.jsx       # Company dashboard
│   │   │   ├── AddJob.jsx          # Create new job posting
│   │   │   ├── ManageJobs.jsx      # Company's job listings
│   │   │   └── ViewApplications.jsx # View applicants for a job
│   │   │
│   │   ├── App.jsx                  # Main app component with routing
│   │   ├── main.jsx                 # React entry point
│   │   └── index.css                # Global styles + Tailwind imports
│   │
│   ├── .env                         # Environment variables (CLIENT)
│   ├── package.json                 # Frontend dependencies
│   ├── vite.config.js               # Vite configuration
│   ├── tailwind.config.js           # Tailwind CSS configuration
│   ├── vercel.json                  # Vercel deployment config
│   └── README.md
│
├── server/                          # Backend Node.js Application
│   ├── config/
│   │   ├── db.js                   # MongoDB connection setup
│   │   ├── cloudinary.js           # Cloudinary SDK configuration
│   │   ├── multer.js               # File upload middleware config
│   │   └── instrument.js           # Sentry error tracking setup
│   │
│   ├── controller/                  # Request handlers (business logic)
│   │   ├── userController.js       # User profile & applications
│   │   ├── jobController.js        # Job CRUD operations
│   │   ├── comapanyController.js   # Company auth & management
│   │   └── webhooks.js             # Clerk user sync webhooks
│   │
│   ├── middleware/
│   │   └── authMiddleware.js       # JWT verification for companies
│   │
│   ├── models/                      # MongoDB Mongoose schemas
│   │   ├── User.js                 # User profile schema
│   │   ├── Company.js              # Company profile schema
│   │   ├── Job.js                  # Job posting schema
│   │   └── JobApplication.js       # Application schema
│   │
│   ├── routes/                      # API route definitions
│   │   ├── userRoutes.js           # /api/users/*
│   │   ├── jobRoutes.js            # /api/jobs/*
│   │   └── companyRoutes.js        # /api/company/*
│   │
│   ├── utils/
│   │   └── generateToken.js        # JWT token generator
│   │
│   ├── .env                         # Environment variables (SERVER)
│   ├── server.js                    # Express app entry point
│   ├── package.json                 # Backend dependencies
│   └── vercel.json                  # Vercel config (unused - on Render)
│
└── README.md                        # This file
```

---

## 🚀 Getting Started

### Prerequisites
Ensure you have the following installed:
- **Node.js** (v18 or higher) - [Download](https://nodejs.org/)
- **npm** or **yarn** - Comes with Node.js
- **Git** - [Download](https://git-scm.com/)
- **MongoDB Atlas Account** - [Sign up](https://www.mongodb.com/cloud/atlas)
- **Clerk Account** - [Sign up](https://clerk.com/)
- **Cloudinary Account** - [Sign up](https://cloudinary.com/)

---

### 📦 Installation

#### 1️⃣ Clone the Repository
```bash
git clone https://github.com/yourusername/job-portal.git
cd job-portal
```

#### 2️⃣ Install Backend Dependencies
```bash
cd server
npm install
```

#### 3️⃣ Install Frontend Dependencies
```bash
cd ../client
npm install
```

---

### ⚙️ Environment Variables

#### **Backend (server/.env)**
Create a `.env` file in the `server/` directory:

```env
# MongoDB Atlas
MONGODB_URI=mongodb+srv://username:password@cluster0.xxxxx.mongodb.net/

# JWT Secret (generate with: node -e "console.log(require('crypto').randomBytes(32).toString('hex'))")
JWT_SECRET=your_64_character_secret_key_here

# Cloudinary
CLOUDINARY_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_SECRET_KEY=your_cloudinary_api_secret

# Clerk Authentication
CLERK_PUBLISHABLE_KEY=pk_test_xxxxxxxxxxxxxxxxxxxxx
CLERK_SECRET_KEY=sk_test_xxxxxxxxxxxxxxxxxxxxx
CLERK_WEBHOOK_SECRET=whsec_xxxxxxxxxxxxxxxxxxxxx

# Sentry (Error Tracking - Optional)
SENTRY_DSN=https://xxxxx@xxxxxx.ingest.sentry.io/xxxxx

# Server Port
PORT=5000
```

#### **Frontend (client/.env)**
Create a `.env` file in the `client/` directory:

```env
# Clerk Authentication
VITE_CLERK_PUBLISHABLE_KEY=pk_test_xxxxxxxxxxxxxxxxxxxxx

# Backend API URL (NO trailing /api)
VITE_BACKEND_URL=http://localhost:5000
```

---

### 🏃‍♂️ Running Locally

#### Start Backend Server
```bash
cd server
npm run server    # Uses nodemon for auto-reload
```
Backend will run on `http://localhost:5000`

#### Start Frontend Development Server
```bash
cd client
npm run dev       # Vite dev server
```
Frontend will run on `http://localhost:5173`

---

## 📡 API Documentation

### Base URL
```
Production: https://job-portal-ordg.onrender.com
Local: http://localhost:5000
```

### Authentication
- **Users:** Authenticated via Clerk SDK (Bearer token in `Authorization` header)
- **Companies:** JWT token in `token` header

---

### 🔐 User Endpoints

#### **GET** `/api/users/user`
Get authenticated user profile
```bash
Headers: Authorization: Bearer <clerk_token>
Response: { success: true, user: {...} }
```

#### **POST** `/api/users/apply`
Apply for a job
```bash
Headers: Authorization: Bearer <clerk_token>
Body: { jobId: "..." }
Response: { success: true, message: "Applied Successfully" }
```

#### **GET** `/api/users/applications`
Get user's job applications
```bash
Headers: Authorization: Bearer <clerk_token>
Response: { success: true, applications: [...] }
```

#### **POST** `/api/users/update-resume`
Upload/update user resume
```bash
Headers: Authorization: Bearer <clerk_token>
Body: FormData with 'resume' file
Response: { success: true, message: "Resume Updated Successfully" }
```

---

### 💼 Job Endpoints

#### **GET** `/api/jobs`
Get all visible jobs
```bash
Response: { success: true, jobs: [...] }
```

#### **GET** `/api/jobs/:id`
Get single job by ID
```bash
Response: { success: true, job: {...} }
```

---

### 🏢 Company Endpoints

#### **POST** `/api/company/register`
Register a new company
```bash
Body: FormData {
  name: string,
  email: string,
  password: string,
  image: file
}
Response: { success: true, company: {...}, token: "..." }
```

#### **POST** `/api/company/login`
Company login
```bash
Body: { email: string, password: string }
Response: { success: true, company: {...}, token: "..." }
```

#### **GET** `/api/company/company`
Get authenticated company profile
```bash
Headers: token: <jwt_token>
Response: { success: true, company: {...} }
```

#### **POST** `/api/company/post-job`
Create new job posting
```bash
Headers: token: <jwt_token>
Body: {
  title: string,
  description: string,
  location: string,
  salary: number,
  level: string,
  category: string
}
Response: { success: true, newJob: {...} }
```

#### **GET** `/api/company/list-jobs`
Get company's posted jobs
```bash
Headers: token: <jwt_token>
Response: { success: true, jobsData: [...] }
```

#### **GET** `/api/company/applicants`
Get all applicants for company's jobs
```bash
Headers: token: <jwt_token>
Response: { success: true, applications: [...] }
```

#### **POST** `/api/company/change-status`
Update application status
```bash
Headers: token: <jwt_token>
Body: { id: string, status: "Accepted" | "Rejected" }
Response: { success: true, message: "Status Changed" }
```

#### **POST** `/api/company/change-visibility`
Toggle job visibility
```bash
Headers: token: <jwt_token>
Body: { id: string }
Response: { success: true, job: {...} }
```

---

### 🔗 Webhook Endpoint

#### **POST** `/webhooks`
Clerk user sync webhook
```bash
Headers: svix-id, svix-timestamp, svix-signature
Body: Clerk webhook payload
Events: user.created, user.updated, user.deleted
```

---

## 🌐 Deployment

### Frontend Deployment (Vercel)

1. **Connect GitHub Repository**
   - Go to [Vercel Dashboard](https://vercel.com/dashboard)
   - Import your repository
   - Select the `client` directory as root

2. **Configure Environment Variables**
   ```
   VITE_CLERK_PUBLISHABLE_KEY=pk_test_...
   VITE_BACKEND_URL=https://job-portal-ordg.onrender.com
   ```

3. **Build Settings**
   - Framework Preset: `Vite`
   - Build Command: `npm run build`
   - Output Directory: `dist`
   - Root Directory: `client`

4. **Deploy** - Vercel will auto-deploy on every Git push

---

### Backend Deployment (Render)

1. **Create New Web Service**
   - Go to [Render Dashboard](https://dashboard.render.com/)
   - Connect your GitHub repository
   - Select the `server` directory

2. **Configure Service**
   - Environment: `Node`
   - Build Command: `npm install`
   - Start Command: `npm start`
   - Root Directory: `server`

3. **Add Environment Variables** (All 10 variables from backend .env)

4. **Deploy** - Render will auto-deploy on Git push

---

### Post-Deployment Checklist
- ✅ Update Clerk redirect URLs
- ✅ Add production domains to CORS whitelist in `server.js`
- ✅ Test all API endpoints
- ✅ Verify Cloudinary uploads work
- ✅ Test Clerk authentication flow
- ✅ Check MongoDB Atlas network access

---

## 📊 GTM Strategy

### 🎯 Target User Base

#### **User Personas**

1. **Job Seekers (Primary)**
   - Age: 22-35
   - Tech-savvy freshers and experienced professionals
   - Looking for remote/hybrid opportunities
   - Active on LinkedIn, Naukri, AngelList

2. **Startups & SMEs (Primary)**
   - 10-100 employee companies
   - Fast-growing tech startups
   - Need quick, quality hiring
   - Budget-conscious

3. **HR Managers (Secondary)**
   - Corporate recruiters
   - Agencies posting on behalf of clients
   - Need ATS-like features

---

### 📅 3-Month Roadmap to 10,000 Users

#### **Month 1: Foundation (0 → 500 users)**
**Week 1-2:**
- ✅ Launch MVP on Product Hunt, Hacker News
- ✅ Post on Reddit (r/forhire, r/webdev, r/cscareerquestions)
- ✅ Cold outreach to 50 startups via LinkedIn
- ✅ Create content: "Top 10 Remote Jobs This Week"

**Week 3-4:**
- ✅ Referral program: Invite 3 friends → Get premium free
- ✅ Guest post on Medium, Dev.to (SEO traffic)
- ✅ Partner with 3 coding bootcamps for student access

**KPIs:** 500 signups, 100 job posts, 50 applications

---

#### **Month 2: Growth (500 → 3,000 users)**
**Week 5-6:**
- ✅ Launch Instagram/Twitter with job tips & success stories
- ✅ Email campaign: Weekly curated job digest
- ✅ Community building: Discord server for job seekers
- ✅ WhatsApp groups for niche roles (Frontend, Backend, DevOps)

**Week 7-8:**
- ✅ Influencer partnerships: Tech YouTubers for shoutouts
- ✅ SEO optimization: Target "remote developer jobs India"
- ✅ College campus ambassadors (5 tier-1 colleges)
- ✅ Quora/Stack Overflow engagement

**KPIs:** 3,000 signups, 500 job posts, 1,000 applications

---

#### **Month 3: Scale (3,000 → 10,000 users)**
**Week 9-10:**
- ✅ Paid ads: Google Ads (₹2,500) + Facebook (₹2,500)
- ✅ Job aggregation: Scrape public boards & post
- ✅ AI feature launch: Resume builder + ATS score checker
- ✅ Press coverage: Submit to TechCrunch, YourStory

**Week 11-12:**
- ✅ Webinar series: "How to crack tech interviews"
- ✅ Corporate tie-ups: Offer enterprise plans
- ✅ Mobile app beta launch (React Native)
- ✅ User-generated content: Success story videos

**KPIs:** 10,000 signups, 2,000 job posts, 5,000 applications

---

### 💰 Marketing Plan with ₹5,000 Budget

| Channel | Budget | Strategy | Expected Reach |
|---------|--------|----------|----------------|
| **Google Ads** | ₹2,500 | "Remote jobs India" keyword bidding | 5,000 clicks |
| **Facebook/Instagram** | ₹2,000 | Job seeker + recruiter targeting (22-35) | 50,000 impressions |
| **Influencer Shoutouts** | ₹500 | Micro-influencers in tech/career niche | 10,000 views |
| **Free Channels** | ₹0 | Social media, content, SEO, communities | 100,000+ organic |

---

### 💵 Revenue Streams

#### **1. Freemium Model**
- **Free Tier:** 3 job applications/month, basic profile
- **Pro Tier (₹150/month):**
  - Unlimited applications
  - Resume review by AI
  - Priority in applicant list
  - Analytics dashboard
- **Expected Revenue:** 500 users × ₹150 = ₹75,000/month

#### **2. Company Subscriptions**
- **Starter (₹999/month):** 5 job posts/month
- **Growth (₹2,999/month):** 20 posts + featured listings
- **Enterprise (₹9,999/month):** Unlimited + ATS integration
- **Expected Revenue:** 100 companies × ₹2,000 avg = ₹2,00,000/month

#### **3. Featured Job Listings**
- ₹500/post for 7-day top placement
- Expected Revenue: 50 posts/month × ₹500 = ₹25,000/month

#### **4. Resume Services**
- AI Resume Builder: ₹99 one-time
- Professional Review: ₹499 one-time
- Expected Revenue: 200 users/month × ₹200 avg = ₹40,000/month

**Total Projected Revenue (Month 3):** ₹3,40,000/month

---

## 🗺 Future Roadmap

### Phase 1: AI Enhancements (Next 3 Months)
- 🤖 **Job Matching Algorithm**
  - NLP-based skill extraction from resumes
  - Automated match score calculation
  - Smart job recommendations

- 📊 **Resume Analysis**
  - ATS compatibility checker
  - Keyword optimization suggestions
  - Industry benchmark comparisons

- 💬 **AI Interview Prep**
  - Mock interview bot
  - Answer quality scoring
  - Personalized improvement tips

---

### Phase 2: Web3 Integration (Months 4-6)
- 🔗 **Wallet Connection**
  - MetaMask/Phantom integration
  - Profile wallet address display
  - Optional wallet-based login

- 💰 **Blockchain Payments**
  - Platform fee in SOL/ETH/MATIC
  - Smart contract-based escrow for freelance
  - Crypto salary options

- 🏆 **NFT Certifications**
  - Skill verification badges as NFTs
  - Employer-issued completion certificates
  - Tradable reputation tokens

---

### Phase 3: Platform Expansion (Months 7-12)
- 📱 **Mobile Apps**
  - iOS + Android (React Native)
  - Push notifications for job matches
  - In-app chat with recruiters

- 🌍 **Internationalization**
  - Multi-language support
  - Currency localization
  - Country-specific job boards

- 🤝 **B2B Features**
  - White-label solutions
  - API access for job boards
  - Integration with HRMS platforms

- 🎓 **Learning Platform**
  - Skill courses marketplace
  - Certifications tied to job requirements
  - Employer-sponsored training

---

### Fundraising Strategy

#### **Seed Round Target: $500K**

**Use of Funds:**
- Product Development (40%): AI, mobile app, Web3
- Marketing & Growth (35%): User acquisition, brand
- Operations (15%): Team hiring (5 members)
- Legal & Compliance (10%): Data privacy, contracts

**Pitch Deck Highlights:**
- 📈 Proven traction: 10K users in 3 months
- 💰 Clear revenue model: ₹3.4L MRR
- 🚀 TAM: $200B global recruitment market
- 🔥 Unique angle: AI + Web3 in job matching
- 👥 Founding team expertise in tech + hiring

---

## 🤝 Contributing

We welcome contributions! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Code Style
- Follow ESLint rules (see `.eslintrc`)
- Use Prettier for formatting
- Write meaningful commit messages

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- **Clerk** - Authentication infrastructure
- **MongoDB Atlas** - Database hosting
- **Cloudinary** - Media management
- **Vercel & Render** - Deployment platforms
- **Tailwind CSS** - UI styling framework
- **React Community** - Open-source libraries

---

## 📞 Contact

**Developer:** NANI 


---

<div align="center">

### ⭐ Star this repo if you found it helpful!

**Built with ❤️ for the RizeOS Core Team Internship Assessment**

[Report Bug](https://github.com/yourusername/job-portal/issues) • [Request Feature](https://github.com/yourusername/job-portal/issues) • [Documentation](https://github.com/yourusername/job-portal/wiki)

</div>
