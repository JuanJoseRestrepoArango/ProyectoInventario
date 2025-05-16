
# 📝 Hoja de Requisitos – Proyecto Ecommerce + IA con Laravel + Filament

---

## 🧱 1. Requisitos Generales

* Framework: Laravel 11+
* Panel administrativo: Filament
* Base de datos: MySQL o PostgreSQL
* Frontend: TailwindCSS + Vue.js / React (a elección)
* Infraestructura: Docker o Laravel Sail (opcional), GitHub + GitHub Actions (CI/CD)
* AI: Integración con GPT API o modelos personalizados (por ejemplo para recomendación, chatbot o análisis)

---

### 📦 2. Módulos del Proyecto

#### 2.1. **Autenticación y Gestión de Usuarios**

* Registro e inicio de sesión (clientes y administradores)
* Recuperación de contraseña
* Panel de usuario con historial de pedidos
* Roles y permisos con Spatie (para admins)

#### 2.2. **Gestión de Productos (Filament)**

* CRUD de productos (nombre, imagen, descripción, precio, inventario)
* Categorías y subcategorías
* Variantes (talla, color)
* Marcas
* Imágenes múltiples

#### 2.3. **Gestión de Pedidos (Filament + Cliente)**

* Carrito de compras
* Checkout (datos de envío, pago simulado)
* Estados del pedido (pendiente, enviado, entregado)
* Gestión de stock al comprar

#### 2.4. **Frontend estilo Shopify**

* Página de inicio con destacados
* Vista de productos por categoría
* Detalle de producto
* Carrito y checkout
* Página de contacto

#### 2.5. **IA (opciones a elegir e implementar)**

* **Chatbot con IA (GPT)** para atención al cliente
* **Recomendaciones de productos** basadas en historial de usuario
* **Auto-descripción de productos** desde imágenes o input (opcional)
* **Análisis de comentarios de clientes** con resumen automático

---

### ⚙️ 3. Requisitos Técnicos

#### Backend (Laravel)

* Eloquent ORM
* Migrations, Seeders, Factories
* API REST (si el frontend se conecta por Vue/React)
* Validaciones, políticas de acceso

#### Admin (Filament)

* Recursos: Productos, Pedidos, Usuarios, Categorías
* Widgets: Ventas por mes, productos más vendidos
* Notificaciones: pedidos nuevos
* Dashboard personalizable

#### Frontend (Vue o React o Blade)

* UI responsiva con TailwindCSS
* Conexión a API (Axios, Fetch o Inertia.js si se usa Vue)
* Componente reutilizables (cards, botones, layouts)

#### IA (OpenAI o alternativa)

* Uso de API Key segura
* Almacenamiento de prompts y respuestas
* Scripts para recomendaciones (con historial de compra)
* Integración de chatbot con frontend (Widget o modal)

---

### 📋 Repartición de Tareas por Persona (Sugerido para 3 personas)

#### 👤 Persona 1 – Backend & Base del Proyecto

* Crear el proyecto Laravel y configurar entorno
* Autenticación y roles
* Modelos: Usuario, Producto, Pedido, Categoría
* API REST para frontend
* Checkout y lógica de pedidos

#### 👤 Persona 2 – Filament (Admin)

* Configurar Filament y recursos (CRUD)
* Gestión de productos y categorías
* Panel de pedidos
* Dashboard con widgets
* Seguridad y control de acceso

#### 👤 Persona 3 – Frontend + IA

* Página de inicio, catálogo y detalle de producto
* Carrito y checkout (con llamada a API)
* Integración con IA (Chatbot o Recomendaciones)
* Diseño responsive tipo Shopify
* Documentación de uso IA

---

### ✅ Extras y Mejoras Futuras

* Pasarela de pago real (Stripe o PayPal)
* Multi-idioma y localización
* Sistema de cupones o descuentos
* Opiniones y calificaciones
* Administración de envíos

---
