# 💳 AlkeWallet — Evaluación Módulo 3

Evolución del proyecto **AlkeWallet**, una billetera digital desarrollada en Java. Este módulo incorpora la capa de persistencia con base de datos relacional, gestionando cuentas y transacciones mediante SQL.

![Java](https://img.shields.io/badge/Java-17-blue?logo=openjdk) ![SQL](https://img.shields.io/badge/SQL-Database-orange?logo=mysql) ![Maven](https://img.shields.io/badge/Maven-3.x-orange?logo=apachemaven)

---

## 📋 Descripción

AlkeWallet Módulo 3 añade persistencia al sistema de billetera digital. El modelo de datos incluye usuarios, cuentas y transacciones, con consultas SQL para las operaciones de negocio: consulta de saldo, transferencias, historial de movimientos y gestión de usuarios.

### Funcionalidades
- Registro y gestión de usuarios
- Creación de cuentas con saldo inicial
- Transferencias entre cuentas con validación de saldo
- Historial de transacciones por usuario
- Consultas SQL optimizadas para las operaciones CRUD

---

## 🏗️ Estructura del proyecto

```
Alkewallet-EvaluacionModulo3/
├── alkewallet.sql              # Script DDL/DML: esquema y datos de prueba
├── CarloGonzalezEvaluacionM3.docx  # Documentación de la evaluación
└── LICENSE
```

---

## 🛠️ Tecnologías

| Herramienta | Rol |
|---|---|
| Java 17 | Lógica de negocio |
| SQL (MySQL/PostgreSQL) | Capa de persistencia |
| Maven | Gestión de dependencias |

---

## 🚀 Cómo ejecutar

### Prerrequisitos
- Java JDK 17+
- MySQL o PostgreSQL instalado
- Maven 3.x

### Configurar la base de datos

```bash
# 1. Clonar el repositorio
git clone https://github.com/Carl0gonzalez/Alkewallet-EvaluacionModulo3.git
cd Alkewallet-EvaluacionModulo3

# 2. Crear la base de datos e importar el esquema
mysql -u root -p < alkewallet.sql
# O en PostgreSQL:
psql -U postgres -f alkewallet.sql

# 3. Compilar y ejecutar el proyecto
mvn clean compile
mvn exec:java -Dexec.mainClass="com.alkewallet.App"
```

---

## 📊 Modelo de datos

```
USUARIOS
  id | nombre | email | contraseña

CUENTAS
  id | usuario_id | saldo | moneda

TRANSACCIONES
  id | cuenta_origen_id | cuenta_destino_id | monto | fecha | tipo
```

---

## 💡 Aprendizajes clave

- Diseño de modelo relacional para sistemas financieros
- Implementación de CRUD con JDBC o JPA
- Manejo de transacciones y consistencia de datos (atomicidad)
- Validación de saldo antes de ejecutar transferencias
- Consultas SQL con JOIN para reportes de movimientos

---

## 🔗 Proyectos relacionados

- [AlkeWallet Módulo 2](https://github.com/Carl0gonzalez/Alkewallet-EvaluacionModulo2) — Versión con lógica de negocio en Java
- [AlkeWallet Evaluación General](https://github.com/Carl0gonzalez/AlkewalletEvaluacionGeneral) — Versión móvil en Kotlin/Android

---

## 👤 Autor

**Carlo González** — [GitHub](https://github.com/Carl0gonzalez)
