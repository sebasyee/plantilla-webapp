# React + TypeScript + Vite

This template provides a minimal setup to get React working in Vite with HMR and some Oxlint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Oxc](https://oxc.rs)
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/)

## React Compiler

The React Compiler is not enabled on this template because of its impact on dev & build performances. To add it, see [this documentation](https://react.dev/learn/react-compiler/installation).

## Expanding the Oxlint configuration

If you are developing a production application, we recommend enabling type-aware lint rules by installing `oxlint-tsgolint` and editing `.oxlintrc.json`:

```json
{
  "$schema": "./node_modules/oxlint/configuration_schema.json",
  "plugins": ["react", "typescript", "oxc"],
  "options": {
    "typeAware": true
  },
  "rules": {
    "react/rules-of-hooks": "error",

Cómo utilizar la plantilla para un proyecto nuevo
Cuando quieras crear una Landing Page (u otro proyecto) nuev0 desde GitHub:

Paso 3.1: Crear el nuevo repositorio desde la plantilla
Ve a tu repositorio plantilla-webapp en GitHub.

Haz clic en el botón "Use this template" y selecciona "Create a new repository".

Ponle el nombre de tu cliente o producto (por ejemplo: landing-zapateria).

Haz clic en "Create repository".

GitHub creará un repositorio nuevo, totalmente independiente y sin el historial de commits anterior.

Paso 3.2: Clonar y empezar a trabajar en tu computadora
Abre tu terminal en la carpeta de proyectos y descarga tu nuevo proyecto:

Bash
# 1. Clonar el nuevo repositorio
git clone https://github.com/TU_USUARIO/landing-zapateria.git

# 2. Entrar a la carpeta del nuevo proyecto
cd landing-zapateria

# 3. Instalar las dependencias (ya que node_modules no se subió)
npm install

# 4. Probar que todo encienda
npm run dev
    "react/only-export-components": ["warn", { "allowConstantExport": true }]
  }
}
```

See the [Oxlint rules documentation](https://oxc.rs/docs/guide/usage/linter/rules) for the full list of rules and categories.
