# ESP32 BackEnd Telemetría - Node js

Este proyecto establece un sistema completo de adquisición de datos usando un **ESP32 con sensor DHT22**, que envía información de **temperatura** y **humedad** hacia un **servidor en Node.js**.  
Los datos se almacenan en **MongoDB**.

---

## Dependencias y Versiones

| Dependencia          | Versión  |
| -------------------- | -------- |
| `Axios`              | `1.13.2` |
| `Bcrypt`             | `6.0.0`  |
| `Cors`               | `2.8.5`  |
| `Dotenv`             | `17.2.3` |
| `Express`            | `5.1.0`  |
| `Express Rate Limit` | `8.7.0`  |
| `Json Web Token`     | `9.0.2`  |
| `Mongoose`           | `8.20.1` |
| `Morgan`             | `1.12.1` |
| `Mqtt`               | `5.14.1` |
| `WebSockets`         | `8.21.3` |

## Características

- Lectura real de datos usando **DHT22** (temperatura y humedad).
- Envío de datos en formato **JSON** mediante HTTP POST.
- Backend en **Node.js + Express**.
- Almacenamiento en **MongoDB** con Mongoose.
- API con:
  - `POST /api/telemetria/guardar-telemetria` → Guarda lectura
  - `GET /api/telemetria/listar-telemetria` → Regresa todos los registros
- ESP32 envía datos cada **3 minutos**.

---

## Configuración de ESLint

Se configuró **ESLint** desde cero utilizando el asistente oficial:

```bash
pnpm create @eslint/config@latest
```

Durante la configuración se seleccionaron las siguientes opciones:

| Opción               | Configuración                   |
| -------------------- | ------------------------------- |
| Código a analizar    | JavaScript                      |
| Uso de ESLint        | Detectar problemas (`problems`) |
| Tipo de módulos      | ESM                             |
| Framework            | Ninguno                         |
| TypeScript           | No                              |
| Entorno de ejecución | Node.js                         |
| Gestor de paquetes   | pnpm                            |

> **Nota:** La configuración se realizó mediante el asistente interactivo de ESLint, tomando como base las características actuales del proyecto y evitando reutilizar una configuración de otro proyecto.

### Dependencias

El asistente instaló las dependencias necesarias:

```text
eslint
@eslint/js
globals
```

Estas dependencias fueron instaladas utilizando `pnpm`.

### Archivo de configuración

Se generó el siguiente archivo en la raíz del backend:

```text
eslint.config.mjs
```

Este archivo contiene la configuración de ESLint utilizando el formato actual basado en **Flat Config**.

### Ejecución de ESLint

Para analizar el código del proyecto:

```bash
pnpm run lint
```

Para analizar el código y aplicar automáticamente las correcciones disponibles:

```bash
pnpm run lint:fix
```

---

## Estructura del Backend

```
├── src
│   ├── config
│   │   └── database.js
│   ├── controller
│   │   └── telemetriac.js
│   ├── models
│   │   └── telemetria.js
│   └── routes
│       └── telemetriaRoute.js
├── .gitignore
├── README.md
├── index.js
├── package-lock.json
└── package.json
```
