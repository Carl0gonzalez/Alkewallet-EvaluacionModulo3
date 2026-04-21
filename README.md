# 💳 AlkeWallet — Evaluación Módulo 3

Evolución de AlkeWallet centrada en la **persistencia relacional**, con un script SQL que modela usuarios, cuentas y transacciones para una billetera digital.

![SQL](https://img.shields.io/badge/SQL-Database-orange?logo=mysql) ![Java](https://img.shields.io/badge/Java-model-lightgrey?logo=openjdk)

---

## 📌 Objetivo

Extender el caso AlkeWallet hacia una base de datos relacional, dejando una estructura inicial para operaciones financieras y consultas de negocio.

## 🧩 Qué incluye

- Script `alkewallet.sql` con estructura de base de datos.
- Documento de evaluación asociado.
- Base para usuarios, cuentas y transacciones.

## 📁 Estructura

```bash
Alkewallet-EvaluacionModulo3/
├── alkewallet.sql
├── CarloGonzalezEvaluacionM3.docx
├── README.md
└── LICENSE
```

## ▶️ Uso

```bash
git clone git@github.com:Carl0gonzalez/Alkewallet-EvaluacionModulo3.git
cd Alkewallet-EvaluacionModulo3
# MySQL
mysql -u root -p < alkewallet.sql
# o PostgreSQL
psql -U postgres -f alkewallet.sql
```

## 💡 Valor del proyecto

Sirve como ejercicio de modelado relacional, persistencia y preparación de estructuras de datos para una aplicación financiera.

## 👤 Autor

**Carlo González**

