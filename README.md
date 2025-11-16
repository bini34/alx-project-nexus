# E-Commerce Project: Customer Mobile App (Flutter) & Admin Web App (Next.js)

---

## Project Overview

This repository implements a **full-stack e-commerce solution** as part of the **ProDev Backend Engineering program** capstone project. The system consists of:

1. **Customer-Facing Mobile App** – Built with **Flutter** for iOS & Android.
2. **Admin Management Web Portal** – Built with **Next.js (React + TypeScript)**.
3. **Backend API** – Powered by **Django REST Framework** with **PostgreSQL** and **JWT authentication**.

The platform supports end-to-end shopping workflows: product browsing, AI-powered recommendations, cart management, **Chapa payment gateway** integration, order tracking, and admin-side inventory, order, and analytics management.

> **Live Demo (Coming Soon)** | **Backend Repo**: [Link TBD] | **Mobile App APK**: [Link TBD]

---

## ProDev Backend Engineering Program Overview

The **ProDev Backend Engineering program** is an intensive, project-driven bootcamp designed to transform learners into production-ready full-stack developers. Through hands-on collaboration between **Frontend** and **Backend** cohorts, participants build real-world applications using modern tools and industry best practices.

### Key Focus Areas:
- **Collaborative Development**: Frontend and Backend learners pair on shared APIs.
- **Real-World Project Delivery**: From ideation to deployment.
- **Agile Workflows**: Git, PR reviews, CI/CD mindset.
- **Cross-Team Communication**: Discord-based coordination via **#ProDevProjectNexus**.

---

## Major Learnings

### Key Technologies Covered
| Domain              | Technologies Used                                      |
|---------------------|--------------------------------------------------------|
| **Mobile Development** | Flutter, Dart, State Management (Provider/Riverpod)   |
| **Web Development**   | Next.js, React, TypeScript, TailwindCSS               |
| **Backend**           | Django REST Framework, PostgreSQL, JWT, Django ORM    |
| **DevOps & Tools**    | Git, GitHub, Postman, Docker (future), CI/CD basics   |
| **Payments**          | Chapa Payment Gateway (Ethiopian fintech)             |

### Important Frontend Development Concepts
- **Next.js App Router** – File-based routing, Server Components, API routes.
- **TailwindCSS** – Utility-first styling, responsive design, dark mode.
- **TypeScript** – Type safety, interfaces for API contracts, reduced runtime errors.
- **System Design & Analysis** – Modular component architecture, state normalization.
- **GraphQL (Explored)** – Compared with REST; used Apollo Client in prototyping.
- **API Integration** – Axios/Fetch wrappers, error handling, loading states, token refresh.

---

## Challenges Faced & Solutions Implemented

| Challenge                              | Solution Implemented                                                                 |
|----------------------------------------|-------------------------------------------------------------------------------------|
| **Cross-platform image rendering in Flutter** | Used `cached_network_image` with placeholder & error widgets; optimized with Yegna CDN. |
| **Real-time order status sync**         | Implemented **Django Channels (WebSocket)** + Flutter StreamBuilder for live updates. |
| **Chapa webhook reliability**           | Added retry logic, idempotency keys, and signature verification using HMAC.         |
| **Admin dashboard performance**         | Server-side rendering in Next.js + pagination + TanStack Query caching.            |
| **Authentication state persistence**    | Secure JWT storage (`flutter_secure_storage`), auto-refresh tokens, interceptors.   |
| **AI Shopping Assistant integration**   | Built prompt-based product recommender using in-stock data + rule-based filtering.  |

---

## Best Practices & Personal Takeaways

### Best Practices Applied
```bash
# Example: Structured Git Workflow
git checkout -b feature/admin-analytics
# → Develop → Test → Commit with clear message
git commit -m "feat: add sales revenue chart with date range filter"
# → Open PR → Request review from backend collaborator
