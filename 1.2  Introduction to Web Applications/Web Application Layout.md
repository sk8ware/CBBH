
---

## 🌐 Web Application Layout 

---

### 🧩 ¿Qué cubre este módulo?

Las aplicaciones web pueden variar muchísimo en estructura, diseño y despliegue. Pero en general, se dividen en 3 categorías clave:

---

### 🏗️ 1. Web Application Infrastructure

Arquitectura física o lógica sobre la que corre una aplicación.

#### Modelos comunes:

|Modelo|Descripción breve|
|---|---|
|**Client-Server**|Arquitectura básica: navegador (cliente) ↔ servidor web (back end)|
|**One Server**|Todo (app + DB) en un solo servidor (riesgoso)|
|**Many Servers - One DB**|Varios servidores acceden a una base de datos compartida|
|**Many Servers - Many DBs**|Cada app tiene su propia DB (mayor seguridad y redundancia)|

✅ Este tipo de segmentación permite contener compromisos y aislar riesgos.

---

### 🧱 2. Web Application Components

Componentes típicos de una app web:

- **Client** (navegador, frontend)
    
- **Server** (backend)
    
- **Webserver** (ej. Nginx, Apache, IIS)
    
- **Lógica de aplicación** (PHP, Python, Node.js…)
    
- **Base de datos** (MySQL, MongoDB…)
    
- **Servicios/Microservicios**
    
- **Integraciones 3rd party**
    
- **Funciones serverless** (AWS Lambda, Azure Functions…)
    

---

### 🧠 3. Web Application Architecture

También llamada **Three-Tier Architecture**:

|Capa|Función principal|
|---|---|
|**Presentación**|UI + JS/CSS/HTML para el cliente (interfaz)|
|**Aplicación**|Procesamiento de lógica, privilegios, reglas del negocio|
|**Datos**|Almacenamiento y recuperación de información (DBs)|

Esta arquitectura puede integrar filtros, controladores, proxys reversos, autenticadores, etc.

---

## ⚙️ Modelos modernos

### 🧬 Microservicios

- Pequeños servicios independientes (ej: login, pagos, reviews)
    
- Comunicación **stateless**
    
- Pueden estar en diferentes lenguajes
    
- ✅ Ventajas: agilidad, reutilización, escalabilidad, resiliencia
    

---

### ☁️ Serverless

- Se ejecuta en contenedores cloud (ej: AWS Lambda)
    
- El proveedor gestiona toda la infraestructura
    
- ✅ Ventajas: sin mantenimiento de servidores, autoscaling, pago por uso
    

---

## 🔐 Arquitectura & Seguridad

Es común que una vulnerabilidad crítica **no esté en el código**, sino en **el diseño de la arquitectura**.

### Ejemplos reales:

|Falla arquitectónica|Impacto|
|---|---|
|Sin RBAC (control de acceso por roles)|Usuarios comunes acceden a funciones de administrador|
|DB en servidor aparte, mal segmentada|Se compromete parcial o totalmente tras RCE|
|Usuarios acceden a datos ajenos|IDOR o falta de separación de lógica entre sesiones|

📌 Estas fallas requieren rediseño, no solo un parche. Por eso es clave hacer **pentests durante todo el ciclo de vida de desarrollo**.

---

### 🧠 Conclusión

Comprender la estructura de una aplicación web:

- Ayuda a **identificar puntos débiles** arquitectónicos
    
- Permite simular ataques reales más precisos
    
- Es vital para pentesters que quieran destacar 🚀
    

---
