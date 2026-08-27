<h1 align="center">Hey, I'm Sergio Martinez Henao </h1>

<h3 align="center">Software Analysis and Development Student | Java · JavaScript · Node.js · SQL</h3>

<p align="center">
  Building REST APIs and Java EE systems, one project at a time, learning along the way.
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/zergioM/zergioM/main/assets/monochair.gif" width="400" />
</p>

---

###  About me

-  Currently studying **Software Analysis and Development (Technologist)** at SENA 
-  I work with **Java EE** (Servlets, JPA/Hibernate) and **Node.js/Express** to build complete applications and REST APIs
-  I like software architecture: separating responsibilities into layers (model, persistence, controller) and keeping code organized and scalable
-  Before moving into development, I worked in logistics — that's where my focus on organization and well-structured processes comes from
-  Constantly learning, also relying on AI tools as part of my workflow
-  Reach me at: [LinkedIn](https://www.linkedin.com/in/sergio-martinezh) · smartinezhenaos@gmail.com

---

###  Technologies & tools

<p align="left">
  <img src="https://skillicons.dev/icons?i=java,js,nodejs,react,mysql,html,css,git,github," />
</p>

---

###  Featured project

####  Jaguar Peak — Retail Management REST API

Retail management system for a chain of stores, built as a complete REST API with **Node.js, Express, and Sequelize**, on top of MySQL/MariaDB. Manages stores, customers, products, employees, and inventory, with authentication and role-based access control.

**🔗 Repository:** [github.com/zergioM/JAGUAR-PEAK-API](https://github.com/zergioM/JAGUAR-PEAK-API)

#### Tech stack
`Express 5` · `Sequelize 6` · `MySQL / MariaDB` · `JWT` · `bcryptjs` · `express-validator` · `helmet` · `cors` · `express-rate-limit` · `morgan`

#### Layered architecture
The project follows a **Controller → Service → Repository → Model** architecture, with strict separation of concerns:

```
src/
├─ routes/         → defines endpoints and applies middlewares
├─ controllers/     → handles the request and builds the response (req/res)
├─ services/         → contains the business logic
├─ repositories/     → the only layer that interacts with the models
├─ models/           → Sequelize entities and relationships
├─ middlewares/       → JWT authentication, roles, field validation
├─ validators/        → validation rules with express-validator
├─ utils/             → response, JWT, and hashing helpers
└─ seeders/           → automatic creation of the admin user
```

#### Key features
- **JWT authentication** — user login and registration, token sent via header (`Authorization: Bearer <token>`)
- **Role-based access control** — create, update, and delete endpoints restricted to the `admin` role; read access available to any authenticated user
- **5 complete CRUD modules**: Stores, Customers, Products, Employees (linked to a Store), and Inventory
- **Inventory alerts** — every inventory record automatically flags low stock (`stock <= minStock`) in the response
- **API security** — `helmet` for secure HTTP headers, configured `cors`, `express-rate-limit` against abuse, passwords hashed with `bcryptjs`
- **Data validation** — per-endpoint input rules with `express-validator`, before reaching the business logic
- **Automatic seeder** — on startup, creates an initial admin user from environment variables

#### Sample endpoint
```
GET /api/inventarios
```
Returns stock by store and product, including `nombreLocal`, `nombreProducto`, `marca`, `categoria`, and a `"STOCK BAJO"` (low stock) alert when applicable.

---

###  Most used languages

<p align="center"> <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=zergioM&layout=compact&theme=default" /> </p>

---

<p align="center"><em>Thanks for visiting my profile 🚀</em></p>
