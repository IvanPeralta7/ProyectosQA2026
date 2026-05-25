# ProyectosQA2026
# 🧪 Cypress QA Automation — Repositorio de Aprendizaje

> 🚀 Proyecto de aprendizaje enfocado en **QA Automation** usando [Cypress](https://www.cypress.io/), cubriendo desde fundamentos hasta casos de prueba avanzados.

---

## 📋 Tabla de Contenidos

- [¿Qué es este repositorio?](#-qué-es-este-repositorio)
- [Tecnologías](#-tecnologías)
- [Estructura del Proyecto](#-estructura-del-proyecto)
- [Instalación](#-instalación)
- [Cómo ejecutar los tests](#-cómo-ejecutar-los-tests)
- [Temario de Aprendizaje](#-temario-de-aprendizaje)
- [Buenas Prácticas](#-buenas-prácticas)
- [Recursos](#-recursos)

---

## 🎯 ¿Qué es este repositorio?

Este repositorio fue creado con el objetivo de aprender **QA Automation** de forma práctica y progresiva usando **Cypress** como herramienta principal. Cada carpeta o archivo representa un concepto clave dentro del mundo del testing automatizado.

Los temas van desde la configuración inicial del entorno hasta patrones avanzados como el **Page Object Model (POM)**, manejo de fixtures, interceptación de requests y más.

---

## 🛠️ Tecnologías

| 🔧 Herramienta | 📌 Versión | 💡 Uso |
|---|---|---|
| 🌲 [Cypress](https://www.cypress.io/) | ^13.x | Framework principal de testing |
| 🟢 [Node.js](https://nodejs.org/) | >=18.x | Entorno de ejecución |
| 🟨 [JavaScript](https://developer.mozilla.org/es/docs/Web/JavaScript) | ES6+ | Lenguaje de los tests |
| ☕ [Mocha](https://mochajs.org/) | integrado | Runner de tests (incluido en Cypress) |
| 🍵 [Chai](https://www.chaijs.com/) | integrado | Librería de assertions |

---

## 📁 Estructura del Proyecto

```
cypress-qa-automation/
│
├── 📂 cypress/
│   ├── 📂 e2e/                    # 🧪 Tests end-to-end organizados por módulo
│   │   ├── 📂 01-fundamentos/     # 🔰 Comandos básicos, selectores y assertions
│   │   ├── 📂 02-formularios/     # 📝 Interacción con inputs, selects, checkboxes
│   │   ├── 📂 03-navegacion/      # 🧭 Rutas, redirecciones, multi-tab
│   │   ├── 📂 04-api-testing/     # 🌐 Requests HTTP con cy.request() e intercept()
│   │   ├── 📂 05-pom/             # 🏗️ Page Object Model pattern
│   │   └── 📂 06-avanzado/        # ⚡ Custom commands, tasks, plugins
│   │
│   ├── 📂 fixtures/               # 📦 Datos estáticos (JSON) para los tests
│   ├── 📂 support/
│   │   ├── 📄 commands.js         # 🔨 Comandos personalizados reutilizables
│   │   └── 📄 e2e.js              # ⚙️ Configuración global antes de cada test
│   │
│   └── 📂 pages/                  # 🗂️ Page Objects (clases por página)
│
├── 📄 cypress.config.js           # ⚙️ Configuración principal de Cypress
├── 📄 package.json
└── 📄 README.md
```

---

## ⚙️ Instalación

### 1️⃣ Clonar el repositorio

```bash
git clone https://github.com/tu-usuario/cypress-qa-automation.git
cd cypress-qa-automation
```

### 2️⃣ Instalar dependencias

```bash
npm install
```

### 3️⃣ Verificar instalación de Cypress

```bash
npx cypress verify
```

---

## ▶️ Cómo ejecutar los tests

### 🖥️ Modo interactivo (GUI de Cypress)

```bash
npx cypress open
```

> 👁️ Permite ver los tests correr en tiempo real en el navegador. Ideal para desarrollo y debugging.

### 💻 Modo headless (línea de comandos)

```bash
npx cypress run
```

### 🎯 Ejecutar un archivo específico

```bash
npx cypress run --spec "cypress/e2e/01-fundamentos/primer-test.cy.js"
```

### 🌐 Ejecutar en un navegador específico

```bash
npx cypress run --browser chrome
npx cypress run --browser firefox
```

---

## 📚 Temario de Aprendizaje

### 🔰 Módulo 1 — Fundamentos
- [ ] 🤔 ¿Qué es Cypress y cómo funciona?
- [ ] 📦 Instalación y configuración del proyecto
- [ ] 🔍 Selectores: `cy.get()`, `cy.contains()`, `cy.find()`
- [ ] ✔️ Assertions básicas con `.should()` y `.expect()`
- [ ] 🖱️ Comandos de acción: `click()`, `type()`, `clear()`, `check()`
- [ ] 🧭 Manejo de la URL: `cy.visit()`, `cy.url()`, `cy.go()`

### 📝 Módulo 2 — Formularios e Interacciones
- [ ] ✏️ Inputs de texto y áreas
- [ ] 🔽 Dropdowns con `cy.select()`
- [ ] ☑️ Checkboxes y radio buttons
- [ ] 📤 Upload de archivos
- [ ] 🔔 Alertas nativas del navegador

### 🧭 Módulo 3 — Navegación y Flujos
- [ ] 🪝 Hooks: `before`, `beforeEach`, `after`, `afterEach`
- [ ] 🌍 Variables de entorno con `Cypress.env()`
- [ ] 🎁 `cy.wrap()` y trabajo con subjects
- [ ] 🏷️ Aliases con `.as()`
- [ ] 🖼️ Manejo de iframes

### 🌐 Módulo 4 — API Testing
- [ ] 📡 `cy.request()` para pruebas de API REST
- [ ] 🕵️ `cy.intercept()` para mockear y espiar requests
- [ ] ✅ Validar respuestas HTTP (status, body, headers)
- [ ] 🔗 Combinación de API + UI en un mismo test

### 🏗️ Módulo 5 — Page Object Model (POM)
- [ ] 🤔 ¿Qué es POM y por qué usarlo?
- [ ] 🧱 Crear clases de página en JavaScript
- [ ] 🔒 Encapsular selectores y acciones
- [ ] ♻️ Reutilización entre tests

### ⚡ Módulo 6 — Avanzado
- [ ] 🔨 Custom Commands en `commands.js`
- [ ] 📦 Fixtures y datos de prueba
- [ ] 🖥️ `cy.task()` para ejecutar código Node.js
- [ ] 📊 Reportes con Mochawesome
- [ ] 🤖 Integración con CI/CD (GitHub Actions)

---

## ✅ Buenas Prácticas

- 🎯 **Usar `data-cy` como selectores** en lugar de clases o IDs de CSS para mayor estabilidad.
  ```html
  <button data-cy="submit-btn">Enviar</button>
  ```
  ```js
  cy.get('[data-cy="submit-btn"]').click()
  ```

- ⏱️ **Evitar `cy.wait()` con tiempos fijos** — usar `cy.intercept()` + `.wait('@alias')` cuando sea posible.

- 🎯 **Un test, una responsabilidad** — cada test debe verificar una sola funcionalidad.

- 🔒 **No depender del estado de otros tests** — cada test debe poder correr de forma independiente.

- 📦 **Usar fixtures para datos de prueba** — evitar hardcodear valores en los specs.

- 🧹 **Limpiar el estado antes de cada test** — usar `beforeEach` para hacer login o preparar el entorno.

---

## 📖 Recursos

| 🔗 Recurso | 📝 Descripción |
|---|---|
| 📘 [Documentación oficial de Cypress](https://docs.cypress.io/) | Referencia completa |
| ✅ [Cypress Best Practices](https://docs.cypress.io/guides/references/best-practices) | Guía de buenas prácticas |
| 🏆 [Testing Trophy - Kent C. Dodds](https://kentcdodds.com/blog/the-testing-trophy-and-testing-classifications) | Estrategia de testing |
| 📗 [The Way of the Web Tester](https://pragprog.com/titles/jrtest/the-way-of-the-web-tester/) | Libro recomendado |
| 🌍 [Cypress Real World App](https://github.com/cypress-io/cypress-realworld-app) | App de ejemplo oficial |

---

## 📝 Notas

💡 Este repositorio está en constante crecimiento a medida que se avanzan los módulos. Cada commit está pensado para reflejar el progreso del aprendizaje, con código comentado y ejemplos claros.

---

<p align="center">
  Hecho con ☕ y muchos <code>cy.get()</code> 🌲✨
</p>
