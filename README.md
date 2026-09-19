# Weather Station


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