#  GestorPro - Sistema de Gestión Integral (Desktop)

**GestorPro** es una solución de escritorio de alto rendimiento diseñada para la administración completa de negocios. Integra un potente motor de backend con una interfaz moderna y fluida, ofreciendo una experiencia de usuario nativa mediante **Electron**.

> [!IMPORTANT]
>  **Estado del Proyecto:** Este sistema se encuentra actualmente en **desarrollo activo**. Recibirá actualizaciones constantes y mejoras de funcionalidades hasta alcanzar su versión de máxima optimización.

---

## 📸 Vista Previa del Sistema

| Acceso al Sistema | Dashboard Principal |
| :---: | :---: |
| <img width="1647" height="1012" alt="gestion3" src="https://github.com/user-attachments/assets/ede3fdf8-c4d9-4423-86fc-d312906f3587" /> | <img width="1597" height="990" alt="gestion2" src="https://github.com/user-attachments/assets/5d5fd8f5-6d82-41e1-a89c-0690ca9f3ef1" />|

| Gestión de Ventas | Metricas |
| :---: | :---: |
| <img width="1193" height="753" alt="gestion1" src="https://github.com/user-attachments/assets/609731c7-cb7f-4807-a99b-a63e9e63a241" /> | <img width="1599" height="1005" alt="gestion4" src="https://github.com/user-attachments/assets/25240aab-0d45-448f-a4ba-23bae5216a0f" /> |

---





## 🛠️ Stack Tecnológico

### Frontend & Desktop
* **Angular 19:** Framework de última generación para la interfaz de usuario.
* **Electron:** Contenedor para ejecutar la web como aplicación nativa de Windows.
* **Angular Material & SweetAlert2:** Componentes UI premium y notificaciones interactivas.

### Backend & API
* **ASP.NET Core (.NET 10):** El núcleo más reciente y rápido para APIs empresariales.
* **Entity Framework Core:** ORM para la gestión de persistencia.
* **PostgreSQL (Neon):** Base de datos relacional alojada en la nube para alta disponibilidad.
* **Seguridad:** Autenticación mediante **JWT** (JSON Web Tokens) y hasheo de claves con **BCrypt**.

---

## 🏛️ Arquitectura del Backend

El backend sigue una **Arquitectura en Capas (N-Layer)** para garantizar escalabilidad y orden:

* **Gestion.App.API:** Capa de entrada (Controllers, Middleware, Program.cs).
* **GestionApp.Business:** Lógica de negocio y procesamiento de servicios.
* **GestionApp.Domain:** Entidades de datos, DTOs y Enums.
* **GestionApp.Infrastructure:** Contexto de base de datos (PostgreSQL), Repositorios y Migraciones.

---

## ✨ Funcionalidades Principales

### 📊 Dashboard & Estadísticas
Visualización en tiempo real de:
* Ganancias del día e ingresos totales.
* Volumen de ventas y cantidad de productos vendidos.
* Gráficos interactivos de rendimiento semanal.

### 👥 Módulo de Clientes (CRUD)
* Registro detallado con DNI, teléfono y correo electrónico.
* Búsqueda inteligente por ID o nombre.
* Historial de compras vinculado automáticamente.

### 📦 Gestión de Inventario
* Control de productos, categorías y stock.
* Actualización automática de existencias tras cada transacción.

### 💰 Punto de Venta (POS)
* Carrito de compras intuitivo.
* Soporte para múltiples métodos de pago: **Efectivo, Tarjeta (Crédito/Débito) y Transferencia**.
* Registro de vendedor (usuario) en cada operación para auditoría.

---

## 🔒 Seguridad de Acceso

Para garantizar la integridad del sistema y el control total por parte del administrador (dueño):
* **Acceso Restringido:** El inicio de sesión es obligatorio mediante credenciales seguras.
* **Gestión Centralizada:** La creación de usuarios nuevos se gestiona directamente desde la base de datos PostgreSQL, asegurando que solo el personal autorizado tenga acceso al software.

---

## 🚀 Instalación y Uso (Usuario Final)

El software se distribuye como un instalador único de Windows, facilitando su despliegue sin necesidad de configuraciones técnicas externas:

1.  Descarga el archivo `setup.exe` desde Release en el repositorio aqui mismo, adjuntar con los otros archivos y darle click al setup`.
2.  Ejecuta el instalador.
3.  El sistema se instalará automáticamente en `Program Files` y generará un **Acceso Directo** en tu escritorio.
4.  ¡Listo! Inicia sesión y comienza a gestionar tu negocio.

---

## 🛠️ Configuración de Desarrollo

Si deseas ejecutar el proyecto localmente:

1.  **Backend:** * Configura tu cadena de conexión en `appsettings.Development.json`.
    * Ejecuta `dotnet ef database update` para replicar las tablas en PostgreSQL.
2.  **Frontend:**
    * Ejecuta `npm install`.
    * Para desarrollo: `npm run electron-dev`.
    * Para generar el instalador: `npm run build:all`.

---
