# 🛒 Friends-Bazaar – MERN Stack E-Commerce Platform

A production-ready full-stack e-commerce web application built using the **MERN Stack** (MongoDB, Express.js, React.js, Node.js). [Friends-Bazaar](https://github.com/PrinceKumar182/Friends-Bazaar) delivers an end-to-end online retail platform featuring secure user authentication, product management, cart persistence, order processing, and administrative controls.

---

## 📌 Product Overview

Local retail stores often face difficulties transitioning online due to complex setups and lack of integrated inventory management. **Friends-Bazaar** provides a streamlined, full-stack digital store platform that bridges local retail catalog management with modern online shopping workflows.

### Key Workflows Solved:
- **Customer Shopping Flow**: Browsing catalog items, managing cart state, checkout, and order history.
- **Admin Management Flow**: Centralized control panel for product creation/updates, inventory tracking, and order status monitoring.
- **Authentication & Security**: Role-based access control protecting administrative endpoints and user order histories.

---

## 🏗️ System Architecture & Data Flow

The platform separates client presentation from backend REST services, serving a pre-built React frontend via Node/Express middleware and interacting with MongoDB for document storage:

```mermaid
flowchart TD
    Client[React.js Client App / Build] <-->|HTTP / REST API| Server[Node.js / Express.js Server]
    
    subgraph Express Backend Layer
        Server --> AuthMW[JWT & Auth Middleware]
        AuthMW --> Controllers[API Controllers]
        Controllers --> Helpers[Helper Functions / BCRYPT]
    end
    
    Controllers <-->|Mongoose ODM| DB[(MongoDB Database)]
