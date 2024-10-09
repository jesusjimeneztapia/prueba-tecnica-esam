# Prueba Técnica ESAM

![Cover](/assets/cover.png)

## Descripción

Crear un componente para renderizar la tarjeta en la imagen, con las siguientes características:

- El componente debe ser reutilizable.
- Debe aceptar las propiedades **título** e **imagen** para que puedan ser asignadas dinámicamente.

## Instalación

### NodeJS

1. Descargar [NodeJS](https://nodejs.org/en/download/package-manager) versión 18.17 o superior.
2. Instalar.

### Proyecto

1. Clonar repositorio `git clone https://github.com/jesusjimeneztapia/prueba-tecnica-esam.git`
2. Ejecute `npm install` para instalar las dependencias del proyecto.
3. Ejecute `npm run dev` para ejecutar el proyecto.
4. Abre el navegador e ingrese a la ruta `http://localhost:4321"`.

### Uso del componente

El componente se llama `CardLink`, el mismo se encuentra en el archivo `src/components/CardLink.astro`.

Tiene las siguientes propiedades:

- **href**, propiedad opcional, que indica la dirección URL a la que el componente redirecciona. Tipo `string`.
- **icon**, propiedad **imagen** de la característica del componente, el mismo indica qué ícono debe renderizarse en el componente, los íconos son de [Material Design Icons](https://pictogrammers.com/library/mdi/). Tipo `string`.
- **title**, propiedad **título** de la característica del componente, el mismo indica qué texto debe renderizar en el componente. Tipo `string`.

Ejemplo de uso básico:

```jsx
<CardLink icon="mdi-account-box-outline" title="perfil personal" />
```

Ejemplo de uso con la propiedad **href**:

```jsx
<CardLink
  href="/perfil-personal"
  icon="mdi-account-box-outline"
  title="perfil personal"
/>
```

> **_Nota:_** En la propiedad **icon** del componente, debe ponerse el nombre del ícono de [Material Design Icons](https://pictogrammers.com/library/mdi/), sin el **mdi** por delante, como se muestra en los ejemplos.

### ¿Por qué Astro?

Al ser una página estática, es decir, que no es una página dinámica en la que los datos dentro de la misma están en constantes cambios, así como no se utiliza el llamado a una API, se decidió usar el framework de Astro, que ayuda justamente en este tipo de páginas, ya que no carga demasiado JavaScript en el cliente, lo cuál lo hace más rápido y ligero. Además se optó por no usar librerías o frameworks como React, Vue, Svelte, entre otros, dentro de Astro, porque no es necesario que los componentes dentro del mismo sean reactivos.

### Librerías utilizadas

Las librearías utilizadas en este proyecto hecho con Astro fueron:

- **@mdi/font**, la misma permite utilizar los íconos de Material Design.
- [Tailwind CSS](https://tailwindcss.com/), es una librería de CSS, se optó por usar esta librería para los estilos del proyecto, porque con la misma se puede crear componentes más rápido, sin preocuparse por crear estilos para cada componente.
- **TypeScript**, una extensión de JavaScript con una sintáxis con tipos.

### Recursos

Se puede ver el proyecto desplegado en la siguiente url: [https://jesusjimenez-pruebatecnicaesam.netlify.app/](https://jesusjimenez-pruebatecnicaesam.netlify.app/)

<br /><br /><br /><br /><br /><br />

# Astro Starter Kit: Basics

```sh
npm create astro@latest -- --template basics
```

[![Open in StackBlitz](https://developer.stackblitz.com/img/open_in_stackblitz.svg)](https://stackblitz.com/github/withastro/astro/tree/latest/examples/basics)
[![Open with CodeSandbox](https://assets.codesandbox.io/github/button-edit-lime.svg)](https://codesandbox.io/p/sandbox/github/withastro/astro/tree/latest/examples/basics)
[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/withastro/astro?devcontainer_path=.devcontainer/basics/devcontainer.json)

> 🧑‍🚀 **Seasoned astronaut?** Delete this file. Have fun!

![just-the-basics](https://github.com/withastro/astro/assets/2244813/a0a5533c-a856-4198-8470-2d67b1d7c554)

## 🚀 Project Structure

Inside of your Astro project, you'll see the following folders and files:

```text
/
├── public/
│   └── favicon.svg
├── src/
│   ├── components/
│   │   └── Card.astro
│   ├── layouts/
│   │   └── Layout.astro
│   └── pages/
│       └── index.astro
└── package.json
```

Astro looks for `.astro` or `.md` files in the `src/pages/` directory. Each page is exposed as a route based on its file name.

There's nothing special about `src/components/`, but that's where we like to put any Astro/React/Vue/Svelte/Preact components.

Any static assets, like images, can be placed in the `public/` directory.

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |

## 👀 Want to learn more?

Feel free to check [our documentation](https://docs.astro.build) or jump into our [Discord server](https://astro.build/chat).
