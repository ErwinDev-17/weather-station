# Weather Station

Weather Station es una **PWA** dedicada a la recolección de datos de un sensor **DHT22** este mismo enviando información mediante conexión Wifi siendo que una backend realizado en **Express** recolecte los datos enviados. La PWA cuenta con envio de datos en tiempo real, registro de logs, acceso de usuarios para administrar información, metricas del sistema, gestíon de usuarios, gráficas de comportamiento de los datos.

## Tecnologías

El proyecto para la recepción de datos enviados desde el dispositovo **ESP32** y el sensor **DHT22** se realizo los siguientes lenguajes y frameworks, para realizar el desarrollo de manera rapida y eficiente.

| Tecnología | Versión |
| --- | --- |
| `Node.js` | `20.20.2` |
| `Angular` | `20.19.3` |
| `C/C++` | `20.19.3` |



### Estructura del Proyecto
```
├── backend
│   ├── src
│   │   ├── config
│   │   ├── controller
│   │   ├── models
│   │   └── routes
│   ├── .gitignore
│   ├── README.md
│   ├── index.js
│   ├── package-lock.json
│   └── package.json
├── firmware
│   ├── main
│   │   ├── cert
│   │   ├── CMakeLists.txt
│   │   └── main.c
│   ├── .gitignore
│   ├── CMakeLists.txt
│   └── README.md
├── frontend
│   ├── public
│   │   ├── icons
│   │   ├── favicon.ico
│   │   └── manifest.webmanifest
│   ├── src
│   │   ├── app
│   │   │   ├── core
│   │   │   │   ├── auth
│   │   │   │   └── graph
│   │   │   ├── pages
│   │   │   │   ├── auth
│   │   │   │   │   ├── login
│   │   │   │   │   ├── register
│   │   │   │   │   └── auth.routes.ts
│   │   │   │   └── graphs
│   │   │   │       ├── home
│   │   │   │       ├── humedity
│   │   │   │       ├── telemetry
│   │   │   │       ├── temperature
│   │   │   │       ├── weather
│   │   │   │       └── graphs.routes.ts
│   │   │   ├── shared
│   │   │   │   ├── components
│   │   │   │   │   ├── footer
│   │   │   │   │   └── sidebar
│   │   │   │   └── shared.module.ts
│   │   │   ├── app.component.css
│   │   │   ├── app.component.html
│   │   │   ├── app.component.spec.ts
│   │   │   ├── app.component.ts
│   │   │   ├── app.config.ts
│   │   │   └── app.routes.ts
│   │   ├── environments
│   │   │   ├── environment.prod.ts
│   │   │   └── environment.ts
│   │   ├── index.html
│   │   ├── main.ts
│   │   └── styles.css
│   ├── .editorconfig
│   ├── .gitignore
│   ├── README.md
│   ├── angular.json
│   ├── ngsw-config.json
│   ├── package-lock.json
│   ├── package.json
│   ├── tsconfig.app.json
│   ├── tsconfig.json
│   └── tsconfig.spec.json
├── .gitignore
└── README.md
```