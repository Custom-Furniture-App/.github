# CustomCraft – Full-Stack Modular E-Commerce & Inventory Management Ecosystem

CustomCraft is a production-ready, multi-platform e-commerce ecosystem designed for custom manufacturing and automated inventory management. The platform allows users to dynamically design, validate, and order modular furniture assets, while providing administrators with rule-based compatibility engines, order fulfillment workflows, and predictive inventory analytics.

## 🌐 System Architecture
The platform is decoupled into three specialized, production-grade repositories:
*   **`frontend-web`** – Admin & Manager ERP Dashboard built with React, Vite, and TypeScript.
*   **`backend-api`** – Secure, high-performance RESTful API engine built with .NET Core and C#.
*   **`mobile-app`** – Cross-platform customer commerce application built with React Native (Expo) and TypeScript.

---

## 🛠️ Core Engineering Features Implemented

### 1. Rule-Based Component Compatibility Engine
*   Developed a dynamic, server-side matrix validation framework in **.NET C#** to enforce real-time component compatibility rules (e.g., matching specific structural frames with validated table-tops).
*   Prevents invalid build configurations on the **React Native** client-side application before payloads hit the checkout workflow.

### 2. Transactional Inventory & Order Lifecycle Management
*   Designed a multi-role fulfillment pipeline handling state transitions across Customers, Assembly Clerks, and Inventory Managers.
*   Implemented thread-safe stock deduction in the backend API to guarantee atomicity during simultaneous checkouts, avoiding overselling during assembly phases.

### 3. Cross-Platform Customer Experience
*   Built a highly responsive consumer app using **React Native (Expo)** featuring dynamic pricing calculators based on live component selections.
*   Integrated global state management to handle customer authentication, profile configurations, and real-time order history tracking.

### 4. Admin ERP & Business Analytics Dashboard
*   Engineered a secure administrative web portal using **Vite React** for real-time inventory management and component performance tracing.
*   Implemented analytics reporting modules that calculate component popularity metrics and inventory turnover rates to assist business stakeholders in demand forecasting.

---

## 🚀 Technical Highlights
*   **End-to-End Type Safety:** Enforced matching TypeScript interfaces on both the Web and Mobile layers against strongly typed C# DTOs on the backend API.
*   **Decoupled Multi-Role Auth:** Designed secure access control ensuring Clerks, Administrators, and Customers only access their respective operational endpoints.
