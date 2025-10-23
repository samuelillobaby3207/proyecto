# 🚀 ReservaYa – Sistema de reservas de citas online con LAMP automatizado

## 📖 Descripción
ReservaYa es una aplicación web que permite a los usuarios registrarse, iniciar sesión y gestionar reservas de citas de manera segura.  
El proyecto integra un entorno **LAMP completo (Linux, Apache, MySQL, PHP)** y permite la automatización del despliegue y administración del sistema mediante **scripts Bash, Ansible y Docker**.  
El objetivo es combinar el desarrollo de una aplicación web funcional con la **configuración, seguridad, monitorización y despliegue**, abordando competencias de varios módulos de ASIR.

---

## 🎯 Objetivos

### Principales
- Configurar y asegurar un entorno **LAMP** en un servidor Linux.  
- Automatizar la instalación y despliegue mediante **scripts Bash o Ansible** (`deploy.sh` o `docker-compose.yml`).  
- Implementar un sistema de **autenticación segura** con sesiones, roles y contraseñas cifradas (bcrypt o Argon2).  
- Gestionar **copias de seguridad automáticas** de la base de datos y logs de la aplicación.  
- Desplegar el sistema en **Docker y en la nube** (AWS o Azure).

### Secundarios
- Configurar **HTTPS** en el servidor Apache.  
- Integrar monitorización básica con herramientas como **phpMyAdmin, Adminer o Netdata**.  
- Añadir **tablas de logs** para registrar accesos y cambios.  
- Explorar la posibilidad de implementar **balanceo o alta disponibilidad**.  
- Documentar procedimientos y pruebas.

---

## 🛠 Tecnologías utilizadas
- **Frontend:** HTML, CSS, JS  
- **Backend:** PHP  
- **Base de datos:** MySQL / MariaDB  
- **Prototipo:** TeleportHQ  
- **Seguridad:** cifrado de contraseñas, validación de formularios  
- **Entorno de desarrollo:** XAMPP, Docker, Docker Compose, VS Code  

---

## 👥 Gestión de usuarios y roles
- **Administrador:** crea servicios, gestiona usuarios y controla reservas.  
- **Proveedor:** opcionalmente puede crear servicios.  
- **Cliente:** reserva citas en servicios disponibles.

### Flujo de reservas
1. El administrador crea los servicios.  
2. El cliente reserva un servicio (fecha y hora disponibles).  
3. El sistema guarda la reserva en la base de datos.  
4. El administrador puede confirmar o cancelar reservas.

---

## 💾 Base de datos y seguridad
- **Quién crea los servicios:** administrador  
- **Quién reserva las citas:** clientes registrados  
- **Seguridad:** cada usuario solo puede acceder a sus propias reservas o a las que puede gestionar según su rol  
- **Mejoras:** tablas de logs para registrar accesos y cambios importantes

---

## 🖥 Entornos de aplicación
**Software:**  
- XAMPP (entorno local)  
- Docker y Docker Compose  
- MySQL / MariaDB  
- phpMyAdmin / Adminer  
- VS Code  

**Hardware recomendado:**  
- PC con Windows 10 o Linux  
- 8 GB RAM  
- 50 GB libres en disco

---

## 🗂 Fases de desarrollo
1. **Planificación:** definir objetivos, alcance y tecnologías  
2. **Diseño:** diagrama de base de datos, roles de usuarios, diseño de servicios y flujo de reservas  
3. **Configuración del servidor:** instalación y configuración de Apache, PHP y MySQL; seguridad y HTTPS  
4. **Desarrollo y pruebas:** scripts PHP para gestión de usuarios, servicios y reservas; pruebas de funcionalidades y seguridad; scripts de automatización (Bash/Ansible)  
5. **Despliegue:** levantar la aplicación en Docker y en la nube (AWS o Azure); inicializar base de datos y copias de seguridad automáticas  
6. **Mantenimiento:** documentación de procedimientos, auditorías de seguridad, backup de bases de datos y mejoras de la aplicación

---

## 📚 Módulos del ciclo formativo relacionados
- Implantación de sistemas operativos: instalación y configuración de servidores Linux  
- Servicios en red y seguridad: administración de servicios web, HTTPS, monitorización y copias de seguridad  
- Seguridad en sistemas informáticos: gestión de usuarios, roles, contraseñas y permisos  
- Bases de datos: creación de tablas, relaciones y consultas SQL, logs de auditoría  
- Gestión de proyectos y documentación técnica: planificación, pruebas y entrega de memoria
