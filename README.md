<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=700&size=30&duration=3500&pause=1000&color=2F81F7&center=true&vCenter=true&width=800&lines=Hi%2C+I'm+Yousef+Rashed+%F0%9F%91%8B;Backend+Software+Engineer;Laravel+%C2%B7+Node.js+%C2%B7+Go;I+build+APIs+that+don't+break+under+load" alt="Typing SVG" />

<p>
  <a href="https://www.linkedin.com/in/yousef-rashed-80286b2a3"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:yosef22363033@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
  <a href="https://github.com/roshdyosf?tab=repositories"><img src="https://img.shields.io/badge/Repositories-181717?style=for-the-badge&logo=github&logoColor=white" alt="Repositories"/></a>
  <img src="https://komarev.com/ghpvc/?username=roshdyosf&label=Profile%20views&color=2F81F7&style=for-the-badge" alt="Profile views"/>
</p>

</div>

---

## 👨‍💻 About Me

I'm a **backend software engineer** who enjoys the hard parts of server-side work: **concurrency, data consistency, secure authentication, and clean architecture**. I build RESTful APIs with **Laravel** and **Node.js**, I've built services in **Go**, and I care about the details that make a system trustworthy: atomic operations, idempotent payments, rate limiting, and tests that actually try to break things.

- 🔒 Security: OAuth 2.0, JWT, 2FA, Passkeys (WebAuthn), RBAC, policies
- ⚡ Concurrency: Redis Lua scripts, distributed locking, row-level locking, ordered locks to avoid deadlocks
- 🧱 Architecture: Domain-Driven Design, Clean Architecture, service layers, event-driven systems
- 💳 Integrations: Stripe, Zoho CRM, WooCommerce, Cloudinary, Apache Kafka
- ✅ Quality: Pest / PHPUnit, PHPStan (Larastan), Laravel Pint, GitHub Actions CI

---

## 🛠️ Tech Stack

<div align="center">

**Languages**

<img src="https://skillicons.dev/icons?i=php,js,ts,go,cs,postgres&perline=10" alt="Languages"/>

**Backend and Databases**

<img src="https://skillicons.dev/icons?i=laravel,nodejs,express,postgres,mysql,mongodb,redis,kafka&perline=10" alt="Backend and databases"/>

**Frontend Exposure**

<img src="https://skillicons.dev/icons?i=vue,tailwind,html,css&perline=10" alt="Frontend"/>

**DevOps and Tools**

<img src="https://skillicons.dev/icons?i=docker,git,github,githubactions,postman,linux&perline=10" alt="DevOps and tools"/>

</div>

<details>
<summary><b>📚 Full skill breakdown</b></summary>
<br>

| Area | What I work with |
| --- | --- |
| **Languages** | PHP 8, JavaScript (ES6+), TypeScript, Go, SQL, C# |
| **Backend** | Laravel 12/13, Node.js, Express.js, Go (Chi), REST API design, MVC, Clean Architecture, DDD, event-driven architecture, background workers |
| **Data** | PostgreSQL, MySQL, MongoDB (Mongoose), Redis, Eloquent ORM, transactions, row-level locking, query optimization |
| **Concurrency and messaging** | Redis Lua scripts (atomic operations), distributed locking, Apache Kafka (KafkaJS) |
| **Security and auth** | JWT, OAuth 2.0 (Google, Zoho CRM), Sanctum, 2FA, Passkeys (WebAuthn), RBAC, authorization policies, API rate limiting |
| **Integrations and docs** | Stripe, Zoho CRM API, WooCommerce REST API, Cloudinary, OpenAPI (Scramble), Postman |
| **Testing and quality** | Pest, PHPUnit, feature and unit testing, PHPStan (Larastan), Laravel Pint, GitHub Actions |
| **DevOps** | Git, GitHub, Docker, Docker Compose, Render |
| **Frontend exposure** | Vue 3, Inertia.js, Blade, Pug, Tailwind CSS |

</details>

---

## 🚀 Featured Projects

### 🎟️ [High-Concurrency Ticketing API](https://github.com/roshdyosf/high-concurrency-ticketing-api)

> An event-ticketing REST API engineered to **prevent double booking under heavy traffic**.

<img src="https://img.shields.io/badge/Laravel_13-FF2D20?style=flat-square&logo=laravel&logoColor=white"/> <img src="https://img.shields.io/badge/PHP_8.5-777BB4?style=flat-square&logo=php&logoColor=white"/> <img src="https://img.shields.io/badge/PostgreSQL_17-4169E1?style=flat-square&logo=postgresql&logoColor=white"/> <img src="https://img.shields.io/badge/Redis_7-DC382D?style=flat-square&logo=redis&logoColor=white"/> <img src="https://img.shields.io/badge/Stripe-635BFF?style=flat-square&logo=stripe&logoColor=white"/> <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/> <img src="https://img.shields.io/badge/Pest-F28D1A?style=flat-square&logo=pestphp&logoColor=white"/>

- **Atomic multi-seat holds**: a Redis Lua script (all-or-nothing, 10-minute TTL) combined with a conditional PostgreSQL update inside a transaction, with sorted lock ordering to avoid deadlocks.
- **Hybrid seating model**: specific seats or general admission, plus adjacent-seat auto-suggestion.
- **Full spec authored from scratch**: 12 database tables, 45+ endpoints, role permissions, and order and refund state machines.
- **Auth and access control**: Sanctum tokens, email verification, password reset, role-based middleware (customer, organizer, admin), ownership policies, and a global ban middleware that revokes active tokens.
- **Redis-backed rate limiting** per scope: login (per IP and per email), booking, scanning, and public endpoints.
- **Stripe payment lifecycle** *(in active development)*: idempotency keys, signed webhooks with duplicate-event protection, automatic refunds for late payments, and a scheduled job that releases expired holds.
- **Event-scoped gatekeepers, organizer-managed refunds, discount codes, and dynamic QR-code tickets.**
- **130+ Pest tests** (including concurrency scenarios), Larastan level 6, Laravel Pint, and a Docker Compose environment (app, PostgreSQL, Redis, scheduler). Interactive OpenAPI docs via Scramble.

---

### 💰 [Family Eco: Household Finance Tracker](https://github.com/roshdyosf/fEco) &nbsp;·&nbsp; [🌐 Live Demo](https://feco.onrender.com/)

> A shared finance app where families jointly track income, expenses, and balance.

<img src="https://img.shields.io/badge/Laravel_13-FF2D20?style=flat-square&logo=laravel&logoColor=white"/> <img src="https://img.shields.io/badge/Vue_3-4FC08D?style=flat-square&logo=vuedotjs&logoColor=white"/> <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white"/> <img src="https://img.shields.io/badge/Inertia.js-9553E9?style=flat-square&logo=inertia&logoColor=white"/> <img src="https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white"/> <img src="https://img.shields.io/badge/Pest-F28D1A?style=flat-square&logo=pestphp&logoColor=white"/>

- **Family isolation** through an invite-code join system; each family owns its own categories and transactions.
- **Atomic balance updates**: database transactions with row-level locking keep the balance correct under concurrent writes.
- **Complete auth suite**: email verification, password reset, **Google OAuth 2.0**, **two-factor authentication with recovery codes**, and **passkey (WebAuthn) login**.
- **RBAC** with Spatie Laravel Permission (family-head and family-member roles, seven permissions), a service-layer architecture, and Form Request validation.
- **Quality pipeline**: Pest tests, PHPStan, Laravel Pint, and a GitHub Actions CI workflow.

<div align="center">
  <img src="https://github.com/user-attachments/assets/7f1026be-8f0e-4fac-90b4-87cc28e4e857" width="32%" alt="Family Eco dashboard"/>
  <img src="https://github.com/user-attachments/assets/3026c65c-c5c6-4366-9417-29b289f9661b" width="32%" alt="Family Eco screen 2"/>
  <img src="https://github.com/user-attachments/assets/9759935e-20e6-475d-a0b8-01d0b7250392" width="32%" alt="Family Eco screen 3"/>
</div>

---

### 📦 [Product Catalog API (Domain-Driven Design)](https://github.com/roshdyosf/Product-Catalog-DDD) &nbsp;·&nbsp; [🌐 Live API](https://product-catalog-ddd.onrender.com/api/v1/products)

> A microservice organized into strict DDD layers, publishing domain events to Kafka.

<img src="https://img.shields.io/badge/Node.js-5FA04E?style=flat-square&logo=nodedotjs&logoColor=white"/> <img src="https://img.shields.io/badge/Express_5-000000?style=flat-square&logo=express&logoColor=white"/> <img src="https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white"/> <img src="https://img.shields.io/badge/Apache_Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white"/> <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/> <img src="https://img.shields.io/badge/Render-46E3B7?style=flat-square&logo=render&logoColor=black"/>

- **Layered design**: presentation, application, domain, and infrastructure, with repository interfaces and use cases.
- **Event-driven**: publishes `product-created` events to Apache Kafka with KafkaJS.
- **Production-minded API**: filtering, sorting, pagination, field selection, validation, centralized error handling, and rate limiting (100 requests per hour per IP).
- **Shipped**: separate dev and prod Docker Compose files, deployed on Render, with a ready-to-use Postman collection.

---

### 🔄 [Zoho WooCommerce Sync](https://github.com/roshdyosf/zoho-woo-sync)

> An integration that turns WooCommerce orders into Zoho CRM contacts and deals.

<img src="https://img.shields.io/badge/Node.js-5FA04E?style=flat-square&logo=nodedotjs&logoColor=white"/> <img src="https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white"/> <img src="https://img.shields.io/badge/WooCommerce-96588A?style=flat-square&logo=woocommerce&logoColor=white"/> <img src="https://img.shields.io/badge/Zoho_CRM_API_v8-E42527?style=flat-square&logo=zoho&logoColor=white"/> <img src="https://img.shields.io/badge/OAuth_2.0-3C873A?style=flat-square"/>

- Fetches recent WooCommerce orders and authenticates with Zoho CRM through the **OAuth 2.0 refresh-token flow**.
- Creates or resolves a Zoho contact from the customer details, then creates a **deal for each order**.
- Triggered through a single endpoint (`GET /sync-orders`).

---

### 🌍 [NTS: Tour Management and Booking Platform](https://github.com/roshdyosf/ntsPJ)

> A full MVC web app and API for tours, bookings, users, and reviews.

<img src="https://img.shields.io/badge/Node.js-5FA04E?style=flat-square&logo=nodedotjs&logoColor=white"/> <img src="https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white"/> <img src="https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white"/> <img src="https://img.shields.io/badge/Pug-A86454?style=flat-square&logo=pug&logoColor=white"/> <img src="https://img.shields.io/badge/Stripe-635BFF?style=flat-square&logo=stripe&logoColor=white"/> <img src="https://img.shields.io/badge/JWT-000000?style=flat-square&logo=jsonwebtokens&logoColor=white"/>

- MVC backend with **filtering, sorting, pagination, and field limiting**.
- **Stripe** payments and booking management, **JWT** authentication, role-based authorization.
- Mongoose-backed **review and rating system**, data seeding scripts, and API docs (OpenAPI and a static web doc).

---

### 🎓 [MAHD: Content Management and E-Learning Backend](https://github.com/roshdyosf/content-mangement-apis)

> Backend for content and course management, built around Clean Architecture.

<img src="https://img.shields.io/badge/Node.js-5FA04E?style=flat-square&logo=nodedotjs&logoColor=white"/> <img src="https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white"/> <img src="https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white"/>

- **Clean Architecture** decouples business logic from framework dependencies.
- APIs for content and course management and student tracking, with global error-handling middleware.

---

## 📊 GitHub Stats

<div align="center">

<img height="180" src="https://github-readme-stats.vercel.app/api?username=roshdyosf&show_icons=true&theme=tokyonight&hide_border=true&include_all_commits=true&count_private=true" alt="GitHub stats"/>
<img height="180" src="https://github-readme-stats.vercel.app/api/top-langs/?username=roshdyosf&layout=compact&theme=tokyonight&hide_border=true&langs_count=8" alt="Top languages"/>

<img src="https://streak-stats.demolab.com?user=roshdyosf&theme=tokyonight&hide_border=true" alt="GitHub streak"/>

</div>

---

## 🎓 Education and Learning

- **B.Tech in Industrial and Energy Technology** (Computer Science specialization), Faculty of Industrial Technology and Energy, graduated July 2025
- **Full Stack Web Development using Python** (120 hrs), Information Technology Institute (ITI), 2024: OOP, PostgreSQL, Flask, Django
- **Node.js, Express, MongoDB and More: The Complete Bootcamp** (42 hrs), Udemy, 2026
- **AI and Python Fundamentals**, ITIDA

---

## 🤝 Let's Connect

I'm open to **backend engineering** opportunities where I can work on APIs, concurrency, and system design.

<div align="center">

<a href="https://www.linkedin.com/in/yousef-rashed-80286b2a3"><img src="https://img.shields.io/badge/Connect_on_LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
<a href="mailto:yosef22363033@gmail.com"><img src="https://img.shields.io/badge/Send_an_Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white"/></a>

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=110&section=footer" alt="footer"/>

</div>
