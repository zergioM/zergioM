<h1 align="center">Hola, soy Sergio Martínez Henao 👋</h1>

<h3 align="center">Estudiante de Análisis y Desarrollo de Software | Java · JavaScript · Node.js · SQL</h3>

<p align="center">
  Construyendo APIs REST y sistemas Java EE, uno por uno, aprendiendo en el camino.
</p>

---

### 🧑‍💻 Sobre mí

- 🎓 Actualmente cursando **Tecnología en Análisis y Desarrollo de Software** en el SENA 
- 💻 Trabajo con **Java EE** (Servlets, JPA/Hibernate) y **Node.js/Express** para construir aplicaciones y APIs REST completas
- 🏗️ Me gusta la arquitectura de software: separar responsabilidades en capas (modelo, persistencia, controlador) y mantener el código organizado y escalable
- 🔄 Antes de dedicarme al desarrollo, trabajé en logística — de ahí viene mi gusto por la organización y los procesos bien estructurados
- 🌱 Aprendiendo constantemente, apoyándome también en herramientas de IA como parte de mi flujo de trabajo
- 📫 Contáctame: [LinkedIn](https://www.linkedin.com/in/sergio-martinezh) · smartinezhenaos@gmail.com

---

### 🛠️ Tecnologías y herramientas

<p align="left">
  <img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" />
  <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white" />
  <img src="https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white" />
  <img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black" />
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" />
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" />
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" />
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" />
  <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" />
  <img src="https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white" />
  <img src="https://img.shields.io/badge/Maven-C71A36?style=for-the-badge&logo=apachemaven&logoColor=white" />
</p>

---

### 🚀 Proyecto destacado

#### 🏔️ Jaguar Peak — API REST de Gestión de Retail

Sistema de gestión de retail para una cadena de locales, construido como API REST completa con **Node.js, Express y Sequelize**, sobre MySQL/MariaDB. Administra locales, clientes, productos, trabajadores e inventario, con autenticación y control de acceso por roles.

**🔗 Repositorio:** [github.com/zergioM/JAGUAR-PEAK-API](https://github.com/zergioM/JAGUAR-PEAK-API)

#### Stack técnico
`Express 5` · `Sequelize 6` · `MySQL / MariaDB` · `JWT` · `bcryptjs` · `express-validator` · `helmet` · `cors` · `express-rate-limit` · `morgan`

#### Arquitectura en capas
El proyecto sigue una arquitectura **Controller → Service → Repository → Model**, con una separación estricta de responsabilidades:

```
src/
├─ routes/         → define los endpoints y aplica middlewares
├─ controllers/     → recibe la petición y arma la respuesta (req/res)
├─ services/         → contiene la lógica de negocio
├─ repositories/     → única capa que interactúa con los modelos
├─ models/           → entidades Sequelize y relaciones
├─ middlewares/       → autenticación JWT, roles, validación de campos
├─ validators/        → reglas de validación con express-validator
├─ utils/             → helpers de respuesta, JWT y hashing
└─ seeders/           → creación automática del usuario administrador
```

#### Funcionalidades principales
- **Autenticación JWT** — login y registro de usuarios, token enviado por header (`Authorization: Bearer <token>`)
- **Control de acceso por roles** — endpoints de creación, edición y eliminación restringidos a rol `admin`; consulta disponible para cualquier usuario autenticado
- **5 módulos completos con CRUD**: Locales, Clientes, Productos, Trabajadores (asociados a un Local) e Inventario
- **Alertas de inventario** — cada registro de inventario calcula automáticamente si el stock está bajo (`stock <= stockMinimo`) y lo marca en la respuesta
- **Seguridad de la API** — `helmet` para cabeceras HTTP seguras, `cors` configurado, `express-rate-limit` contra abuso de peticiones, contraseñas hasheadas con `bcryptjs`
- **Validación de datos** — reglas de entrada por endpoint con `express-validator`, antes de llegar a la lógica de negocio
- **Seeder automático** — al levantar el proyecto, crea un usuario administrador inicial a partir de variables de entorno

#### Ejemplo de endpoint
```
GET /api/inventarios
```
Devuelve el stock por local y producto, incluyendo `nombreLocal`, `nombreProducto`, `marca`, `categoria` y una alerta `"STOCK BAJO"` cuando corresponde.

---

### 📊 Lenguajes más usados

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=zergioM&layout=compact&theme=default" />
</p>

---

<p align="center"><em>Gracias por visitar mi perfil 🚀</em></p>
