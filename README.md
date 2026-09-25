# 🏠 HogarYA — Sistema de Gestión Inmobiliaria

![Java](https://img.shields.io/badge/Java-17-orange?logo=openjdk)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-4.x-6DB33F?logo=springboot&logoColor=white)
![Spring Data JPA](https://img.shields.io/badge/Spring%20Data-JPA-6DB33F?logo=spring&logoColor=white)
![Thymeleaf](https://img.shields.io/badge/Thymeleaf-005F0F?logo=thymeleaf&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?logo=mysql&logoColor=white)
![Maven](https://img.shields.io/badge/Maven-C71A36?logo=apachemaven&logoColor=white)

> Aplicación web para la gestión integral de una inmobiliaria: propiedades, publicaciones, contratos y facturación, con seguimiento del ciclo de vida de cada operación.

---

## 📋 Descripción

**HogarYA** es un sistema desarrollado como Trabajo Final que permite a una inmobiliaria administrar su negocio desde una única aplicación web.

El sistema permite cargar y publicar propiedades, gestionar propietarios e inquilinos, generar contratos de alquiler o venta, emitir facturas y realizar el seguimiento de personas, ubicaciones y estados de las distintas operaciones.

El proyecto fue construido utilizando una **arquitectura por capas**, aplicando reglas de negocio, validaciones y control de estados en las diferentes entidades.

---

## ✨ Funcionalidades principales

- 🏡 **Propiedades** — alta, baja, modificación y listado, con tipos de propiedad, estados de disponibilidad y validación de duplicados.
- 📢 **Publicaciones** — gestión de avisos y control de publicaciones activas.
- 📄 **Contratos** — creación, modificación y baja de contratos de alquiler o venta.
- 🧾 **Facturación** — emisión y gestión de facturas, medios de pago y estados.
- 👤 **Personas** — administración de propietarios e inquilinos.
- 📍 **Ubicaciones** — gestión de provincias y ciudades.
- 🕒 **Historial de estados** — seguimiento de cambios en propiedades, publicaciones, contratos y facturas.
- ✅ **Validaciones y reglas de negocio** — manejo de errores y excepciones propias de la aplicación.

---

## 🛠️ Tecnologías

| Categoría | Tecnología |
|---|---|
| Lenguaje | Java 17 |
| Framework | Spring Boot |
| Persistencia | Spring Data JPA / Hibernate |
| Vistas | Thymeleaf |
| Base de datos | MySQL |
| Validación | Bean Validation |
| Build | Maven |

---

## 🏗️ Arquitectura

El proyecto utiliza una arquitectura por capas para separar las responsabilidades de la aplicación:

```text
com.desi
│
├── entidades        → Modelos JPA
├── accesoDatos      → Repositories (Spring Data JPA)
├── servicios        → Lógica de negocio
├── presentacion     → Controladores Spring MVC
└── excepciones      → Excepciones de negocio
```

Las vistas se encuentran en:

```text
src/main/resources/templates
```

y son renderizadas mediante **Thymeleaf**.

---

## 📸 Capturas

> Próximamente se agregarán capturas de las principales funcionalidades de la aplicación.

---

## 🚀 Cómo ejecutarlo

### Requisitos

- JDK 17
- MySQL
- Maven o Maven Wrapper

### Pasos

1. Clonar el repositorio:

```bash
git clone https://github.com/Nachitoo321/HogarYA.git
cd HogarYA
```

2. Crear la base de datos en MySQL:

```sql
CREATE DATABASE hogarya;
```

3. Configurar las credenciales de MySQL en:

```text
src/main/resources/application.properties
```

4. Ejecutar la aplicación:

```bash
./mvnw spring-boot:run
```

En Windows:

```bash
mvnw.cmd spring-boot:run
```

La aplicación estará disponible en:

```text
http://localhost:8080
```

---

## 👥 Autores

Trabajo Final desarrollado en equipo:

- **[Ignacio Oroño](https://github.com/Nachitoo321)**
- [Josefina Acevedo](https://github.com/Josefinaac95)
- [David Reigenborn](https://github.com/ReigenbornDavid)
- [Franco Zambuto](https://github.com/FrancoZambuto)

---

## 🎓 Contexto académico

Proyecto desarrollado como parte de la **Tecnicatura Universitaria en Tecnologías de la Información** de la **Universidad Tecnológica Nacional — Facultad Regional Santa Fe**.

> Este repositorio es un fork del proyecto colaborativo original y se conserva como parte de mi portfolio académico.

---

<p align="center">
  Desarrollado como proyecto académico con ☕ Java + Spring Boot 🌱
</p>
