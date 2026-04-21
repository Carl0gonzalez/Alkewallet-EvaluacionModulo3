# 💳 AlkeWallet — Evaluación Módulo 3

Extensión del caso AlkeWallet orientada a la **persistencia relacional**, con un script SQL para modelar usuarios, cuentas y transacciones.

![SQL](https://img.shields.io/badge/SQL-Database-orange?logo=mysql)

## Descripción

Este repositorio se concentra en el diseño de la capa de datos para una billetera digital. El archivo `alkewallet.sql` define la base necesaria para administrar operaciones financieras, historial de movimientos y relaciones entre entidades principales.

## Objetivo

Trasladar la lógica del caso AlkeWallet hacia un modelo relacional que sirva como base para consultas y operaciones persistentes.

## Uso

```bash
# MySQL
mysql -u root -p < alkewallet.sql

# PostgreSQL
psql -U postgres -f alkewallet.sql
```

## Autor

**Carlo González**

