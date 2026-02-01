# 🏘️ Mantiqati - Revolutionary Collective Purchasing Platform

<div align="center">

![Mantiqati Banner](https://img.shields.io/badge/Mantiqati-Community_Shopping-10b981?style=for-the-badge&logo=shopping-cart&logoColor=white)
[![Live Demo](https://img.shields.io/badge/Live-Demo-3b82f6?style=for-the-badge&logo=google-chrome&logoColor=white)](https://moh222salah.github.io/cv)
[![WhatsApp](https://img.shields.io/badge/WhatsApp-Connect-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)](https://wa.me/201113903070)

**Transforming Community Shopping Through Collective Purchasing Power**

Save 40-50% on essential goods by buying directly from wholesalers

[Features](#-key-features) • [Technology](#️-technology-stack) • [Process](#-how-it-works) • [Architecture](#-technical-architecture) • [Contact](#-contact)

</div>

---

## 📋 Table of Contents

- [Overview](#-overview)
- [The Problem](#-the-problem)
- [The Solution](#-the-solution)
- [Key Features](#-key-features)
- [How It Works](#-how-it-works)
- [Technology Stack](#️-technology-stack)
- [Technical Architecture](#-technical-architecture)
- [Impact & Statistics](#-impact--statistics)
- [Roadmap](#-roadmap)
- [Installation](#-installation)
- [Contributing](#-contributing)
- [Contact](#-contact)
- [License](#-license)

---

## 🌟 Overview

**Mantiqati** (Arabic: منطقتي - "My Neighborhood") is a groundbreaking digital platform that empowers communities to achieve massive savings on essential goods through collective purchasing. By leveraging the power of bulk buying, we connect neighbors directly with wholesalers, eliminating retail markup and delivering savings of up to 50%.

### 🎯 Mission

To democratize access to affordable essential goods by building strong, self-sufficient communities that harness collective purchasing power.

### 💡 Vision

A future where every community can access wholesale prices, breaking the monopoly of retail traders and ensuring economic fairness for all families.

---

## 🔴 The Problem

### Current Market Reality

- **Excessive Retail Markup**: Retail prices are often 2x wholesale prices
- **Limited Access**: Individual families cannot access wholesale markets
- **Trader Monopolies**: Small shops control pricing in neighborhoods
- **Financial Burden**: Essential goods consume a disproportionate share of family budgets
- **Lack of Transparency**: Hidden costs and markup percentages

### Impact on Families

```
Average Egyptian Family Budget Impact:
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Monthly Essential Goods: ~1,500 EGP
Annual Cost: 18,000 EGP
Potential Savings with Mantiqati: 8,460 EGP/year
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

---

## ✅ The Solution

### Mantiqati Platform

A mobile-first web application that:

1. **Groups Neighbors** by geographic region
2. **Announces Bulk Deals** (e.g., 1 ton of rice at wholesale price)
3. **Collects Orders** from community members with upfront payment
4. **Purchases Directly** from wholesalers/manufacturers when target is met
5. **Distributes Locally** through trusted volunteer coordinators

### Value Proposition

| Traditional Shopping | Mantiqati Platform |
|---------------------|-------------------|
| 30 EGP/kg (retail) | 16 EGP/kg (wholesale) |
| Individual purchases | Community bulk buying |
| Hidden costs | 100% transparent pricing |
| Retail markup: 50-100% | Direct sourcing: 0% markup |
| Limited choices | Multiple supplier options |

---

## ⚡ Key Features

### 🎯 Core Functionality

#### 1. **Geographic Smart Matching**
```
┌─────────────────────────────────────┐
│  User Opens App                     │
│         ↓                           │
│  GPS Auto-Detection                 │
│         ↓                           │
│  Matched to Region                  │
│         ↓                           │
│  View Active Group Purchases        │
└─────────────────────────────────────┘
```

- Automatic region assignment using GPS/IP geolocation
- PostGIS-powered spatial database queries
- Neighborhood-based grouping for optimal logistics

#### 2. **Real-Time Progress Tracking**

```css
Progress Bar: [████████████░░░░░░░░] 85%
850 kg / 1,000 kg | 170 orders | 2 days left
```

- Live updates as neighbors join
- Visual progress indicators
- Countdown timers to deadline
- Push notifications at key milestones

#### 3. **Transparent Pricing**

```
Supplier Invoice:        16,000 EGP (1,000 kg @ 16 EGP/kg)
Platform Fee (2%):          320 EGP
Transportation:             180 EGP
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Total Cost:             16,500 EGP
Cost per kg:            16.50 EGP
Retail Price:           30.00 EGP
YOUR SAVINGS:           45% (13.50 EGP/kg)
```

#### 4. **Secure Payment System**

- Multiple payment gateways (Fawry, Paymob, Credit Cards)
- Escrow protection - funds held until purchase complete
- Automatic refunds if target not met
- PCI DSS compliant security

#### 5. **Smart Distribution**

- Multiple pickup locations per region
- QR code verification system
- Time slot booking to avoid crowds
- Optional home delivery service

#### 6. **Community Trust System**

- Verified volunteer coordinators
- Rating and review system
- Transparent transaction history
- Quality guarantee on products

---

## 🔄 How It Works

### **4-Step Process**

```
┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓
┃  Step 1: ANNOUNCEMENT                Day 1        ┃
┣━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┫
┃  📢 Product posted (1 ton rice @ 16 EGP/kg)       ┃
┃  🎯 Target: 1,000 kg                              ┃
┃  ⏰ Deadline: 7 days                              ┃
┃  📍 Region: Maadi, Cairo                          ┃
┗━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┛

┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓
┃  Step 2: ORDER & PAY                Days 2-5      ┃
┣━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┫
┃  🛒 Residents place orders (min 5kg)              ┃
┃  💳 Upfront payment via app                       ┃
┃  📊 Progress: 450kg → 700kg → 950kg              ┃
┃  🔔 Notifications: "Only 50kg left!"              ┃
┗━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┛

┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓
┃  Step 3: PURCHASE                    Day 6        ┃
┣━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┫
┃  ✅ Target reached: 1,000 kg                      ┃
┃  📝 Order placed with supplier                    ┃
┃  🚚 Delivery scheduled: 24-48 hours               ┃
┃  📲 All participants notified                     ┃
┗━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┛

┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓
┃  Step 4: DISTRIBUTION                Day 8        ┃
┣━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┫
┃  📍 Pickup at designated locations                ┃
┃  🔍 QR code verification                          ┃
┃  👥 Volunteer coordinators assist                 ┃
┃  ⭐ Rate experience & product quality             ┃
┗━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┛
```

---

## 🛠️ Technology Stack

### **Frontend**

```
┌─────────────────────────────────────────────┐
│  Mobile App                                 │
├─────────────────────────────────────────────┤
│  • React Native / Flutter                   │
│  • Redux Toolkit (State Management)         │
│  • React Navigation                         │
│  • Styled Components                        │
│  • Lottie (Animations)                      │
└─────────────────────────────────────────────┘

┌─────────────────────────────────────────────┐
│  Admin Dashboard                            │
├─────────────────────────────────────────────┤
│  • React.js                                 │
│  • Ant Design / Material-UI                 │
│  • Chart.js / Recharts                      │
│  • React Query                              │
└─────────────────────────────────────────────┘
```

### **Backend**

```
┌─────────────────────────────────────────────┐
│  API Server                                 │
├─────────────────────────────────────────────┤
│  • Node.js + Express / Python + FastAPI     │
│  • JWT Authentication                       │
│  • Socket.io (Real-time)                    │
│  • Rate Limiting & Security                 │
└─────────────────────────────────────────────┘

┌─────────────────────────────────────────────┐
│  Database                                   │
├─────────────────────────────────────────────┤
│  • PostgreSQL 14+ (Primary)                 │
│  • PostGIS (Geospatial)                     │
│  • Redis (Cache & Sessions)                 │
│  • Elasticsearch (Search)                   │
└─────────────────────────────────────────────┘
```

### **Infrastructure & Services**

```
┌─────────────────────────────────────────────┐
│  Cloud & DevOps                             │
├─────────────────────────────────────────────┤
│  • AWS / Google Cloud / Azure               │
│  • Docker + Kubernetes                      │
│  • GitHub Actions (CI/CD)                   │
│  • CloudFlare CDN                           │
└─────────────────────────────────────────────┘

┌─────────────────────────────────────────────┐
│  Third-Party Services                       │
├─────────────────────────────────────────────┤
│  • Google Maps API (Location)               │
│  • Fawry / Paymob (Payments)                │
│  • Firebase FCM (Notifications)             │
│  • Twilio (SMS/OTP)                         │
│  • AWS S3 (Storage)                         │
└─────────────────────────────────────────────┘
```

---

## 🏗️ Technical Architecture

### **System Overview**

```
┌─────────────────────────────────────────────────────────────┐
│                    CLIENT LAYER                             │
├──────────────────┬──────────────────┬──────────────────────┤
│  Mobile App      │  Admin Portal    │  Volunteer App       │
│  (iOS/Android)   │  (Web)           │  (Mobile)            │
└────────┬─────────┴────────┬─────────┴──────────┬───────────┘
         │                  │                    │
         └──────────────────┼────────────────────┘
                            ↓
         ┌──────────────────────────────────────────┐
         │         API GATEWAY                      │
         │  • Load Balancer                         │
         │  • Rate Limiting                         │
         │  • Authentication                        │
         └──────────────────┬───────────────────────┘
                            ↓
         ┌──────────────────────────────────────────┐
         │      APPLICATION LAYER                   │
         ├──────────────────────────────────────────┤
         │  • User Service                          │
         │  • Order Service                         │
         │  • Payment Service                       │
         │  • Location Service                      │
         │  • Notification Service                  │
         └──────────────────┬───────────────────────┘
                            ↓
         ┌──────────────────────────────────────────┐
         │         DATA LAYER                       │
         ├──────────────────────────────────────────┤
         │  PostgreSQL + PostGIS  │  Redis Cache    │
         │  (Primary Database)    │  (Sessions)     │
         └──────────────────────────────────────────┘
```

### **Database Schema (Key Tables)**

```sql
-- Users Table
CREATE TABLE users (
    user_id UUID PRIMARY KEY,
    phone_number VARCHAR(15) UNIQUE,
    full_name VARCHAR(100),
    region_id UUID REFERENCES regions(region_id),
    created_at TIMESTAMP
);

-- Regions Table (with PostGIS)
CREATE TABLE regions (
    region_id UUID PRIMARY KEY,
    region_name VARCHAR(100),
    city VARCHAR(50),
    coordinates POINT,
    polygon GEOMETRY,
    supervisor_id UUID REFERENCES users(user_id)
);

-- Group Purchases Table
CREATE TABLE group_purchases (
    purchase_id UUID PRIMARY KEY,
    region_id UUID REFERENCES regions(region_id),
    product_id UUID REFERENCES products(product_id),
    target_quantity INT,
    current_quantity INT DEFAULT 0,
    price_per_unit DECIMAL(10,2),
    status VARCHAR(20) DEFAULT 'active',
    deadline TIMESTAMP
);

-- Individual Orders Table
CREATE TABLE individual_orders (
    order_id UUID PRIMARY KEY,
    purchase_id UUID REFERENCES group_purchases(purchase_id),
    user_id UUID REFERENCES users(user_id),
    quantity INT,
    total_price DECIMAL(10,2),
    payment_status VARCHAR(20),
    order_status VARCHAR(20)
);
```

### **API Endpoints**

```
Authentication
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
POST   /api/v1/auth/register
POST   /api/v1/auth/login
POST   /api/v1/auth/verify-otp
POST   /api/v1/auth/refresh-token

Users
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
GET    /api/v1/users/profile
PUT    /api/v1/users/profile
GET    /api/v1/users/orders
POST   /api/v1/users/location

Regions
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
GET    /api/v1/regions
GET    /api/v1/regions/:id
GET    /api/v1/regions/nearby
GET    /api/v1/regions/:id/purchases

Group Purchases
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
GET    /api/v1/purchases
GET    /api/v1/purchases/:id
POST   /api/v1/purchases/:id/join
GET    /api/v1/purchases/:id/progress

Orders
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
POST   /api/v1/orders
GET    /api/v1/orders/:id
PUT    /api/v1/orders/:id
POST   /api/v1/orders/:id/payment

Payments
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
POST   /api/v1/payments/initiate
POST   /api/v1/payments/callback
GET    /api/v1/payments/:id/status
POST   /api/v1/payments/:id/refund
```

---

## 📊 Impact & Statistics

### **Projected Impact (Year 1)**

```
┌────────────────────────────────────────────────┐
│  Families Served:           10,000             │
│  Total Savings Generated:   33.6M EGP          │
│  Average Savings/Family:    3,360 EGP/year     │
│  Regions Covered:           50+                │
│  Group Purchases:           2,000+             │
│  Products Available:        100+               │
└────────────────────────────────────────────────┘
```

### **Case Study: Rice Purchase**

| Metric | Retail | Mantiqati | Savings |
|--------|--------|-----------|---------|
| Price per kg | 30 EGP | 16 EGP | 14 EGP (47%) |
| Family order (5kg) | 150 EGP | 80 EGP | 70 EGP |
| Monthly (x4) | 600 EGP | 320 EGP | 280 EGP |
| Annual | 7,200 EGP | 3,840 EGP | **3,360 EGP** |

### **Environmental Impact**

- **Reduced Packaging Waste**: Bulk purchasing = less individual packaging
- **Optimized Logistics**: Single delivery vs. multiple trips to stores
- **Carbon Footprint**: ~40% reduction in transportation emissions

---

## 🗺️ Roadmap

### **Phase 0: Preparation (2 Months)**

- [x] Market research and feasibility study
- [x] Technical architecture design
- [x] Supplier network building
- [ ] Legal entity registration
- [ ] Initial funding secured

### **Phase 1: MVP Launch (3-4 Months)**

- [ ] Develop core mobile app (iOS/Android)
- [ ] Build backend API and database
- [ ] Integrate payment gateway
- [ ] Beta test with 100 users in pilot region
- [ ] Execute 3-5 successful group purchases

**Success Metrics:**
- 100+ active users
- 90%+ purchase completion rate
- 4.5+ app rating
- 45%+ average savings achieved

### **Phase 2: Regional Expansion (6-12 Months)**

- [ ] Add 3-5 new regions in Cairo
- [ ] Scale to 10,000 users
- [ ] Introduce 50+ products
- [ ] Launch marketing campaign
- [ ] Implement 2% platform fee

**Success Metrics:**
- 10,000+ active users
- 50+ active regions
- 100+ group purchases/month
- Break-even operations

### **Phase 3: National Growth (12-24 Months)**

- [ ] Expand to Alexandria, Giza, other major cities
- [ ] Launch B2B service for companies
- [ ] Build dedicated logistics network
- [ ] Introduce premium features
- [ ] Seek Series A funding

**Success Metrics:**
- 100,000+ users
- 200+ regions
- 10M+ EGP monthly GMV
- Profitability achieved

---

## 🚀 Installation

### **Prerequisites**

```bash
Node.js >= 18.0.0
npm >= 9.0.0
PostgreSQL >= 14.0
Redis >= 7.0
Docker (optional but recommended)
```

### **Local Development Setup**

```bash
# Clone the repository
git clone https://github.com/yourusername/mantiqati.git
cd mantiqati

# Install dependencies
npm install

# Set up environment variables
cp .env.example .env
# Edit .env with your configuration

# Set up database
npm run db:migrate
npm run db:seed

# Start development server
npm run dev

# Run tests
npm test
```

### **Docker Setup**

```bash
# Build and run with Docker Compose
docker-compose up -d

# View logs
docker-compose logs -f

# Stop containers
docker-compose down
```

### **Environment Variables**

```env
# Application
NODE_ENV=development
PORT=3000
APP_URL=http://localhost:3000

# Database
DATABASE_URL=postgresql://user:password@localhost:5432/mantiqati
REDIS_URL=redis://localhost:6379

# Authentication
JWT_SECRET=your-super-secret-key
JWT_EXPIRY=24h

# Payment Gateway
FAWRY_MERCHANT_CODE=your-merchant-code
FAWRY_SECURITY_KEY=your-security-key

# Google Maps
GOOGLE_MAPS_API_KEY=your-google-maps-key

# Notifications
FIREBASE_SERVER_KEY=your-firebase-key
TWILIO_ACCOUNT_SID=your-twilio-sid
TWILIO_AUTH_TOKEN=your-twilio-token
```

---

## 🤝 Contributing

We welcome contributions from the community! Here's how you can help:

### **Ways to Contribute**

- 🐛 Report bugs and issues
- 💡 Suggest new features
- 📝 Improve documentation
- 🔧 Submit pull requests
- 🌍 Help with translations
- 🧪 Write and improve tests

### **Development Process**

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### **Code Style**

We follow the [Airbnb JavaScript Style Guide](https://github.com/airbnb/javascript) and use ESLint for enforcement.

```bash
# Run linter
npm run lint

# Fix auto-fixable issues
npm run lint:fix
```

---

## 📞 Contact

### **Developer**

**Mohamed Salah** - Full-Stack Developer

- 💼 **Portfolio**: [moh222salah.github.io/cv](https://moh222salah.github.io/cv)
- 📲 **WhatsApp**: [+20 111 390 3070](https://wa.me/201113903070)
- 📧 **Email**: moh222salah@gmail.com
- 💻 **GitHub**: [@moh222salah](https://github.com/moh222salah)

### **Project Links**

- 🌐 **Live Demo**: [Coming Soon]
- 📖 **Documentation**: [docs.mantiqati.com]
- 🐛 **Issue Tracker**: [GitHub Issues]
- 💬 **Community**: [Discord Server]

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- **Community**: Thanks to all the families and volunteers who participated in our beta testing
- **Advisors**: Economic and technical advisors who guided the project
- **Open Source**: Built with amazing open-source technologies
- **Inspiration**: All the communities worldwide practicing collective economics

---

## 📈 Project Status

```
Current Stage: Development
Version: 0.1.0 (Alpha)
Status: Active Development
Last Updated: February 2026
```

---

<div align="center">

### ⭐ Star this repository if you find it helpful!

**Made with 💚 for Egyptian Communities**

[![GitHub Stars](https://img.shields.io/github/stars/yourusername/mantiqati?style=social)](https://github.com/yourusername/mantiqati)
[![GitHub Forks](https://img.shields.io/github/forks/yourusername/mantiqati?style=social)](https://github.com/yourusername/mantiqati/fork)
[![GitHub Watchers](https://img.shields.io/github/watchers/yourusername/mantiqati?style=social)](https://github.com/yourusername/mantiqati)

---

**Join the revolution. Shop together. Save together.**

[Get Started](#-installation) • [Report Bug](https://github.com/yourusername/mantiqati/issues) • [Request Feature](https://github.com/yourusername/mantiqati/issues)

</div>
