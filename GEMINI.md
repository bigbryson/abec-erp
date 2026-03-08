# Materio - Bootstrap 5 HTML Admin Template

## Project Overview
**Materio** is a comprehensive and responsive Bootstrap 5 HTML Admin Dashboard Template. It is designed to help developers build high-quality, scalable web applications with ease. The project is split into two main directories:

-   **`full-version/`**: The complete template containing all features, UI components, charts, maps, and pre-built pages. Use this for reference or complex applications.
-   **`starter-kit/`**: A lightweight, minimal version of the template. Use this as a clean starting point for new projects to avoid bloat.

## Tech Stack
-   **Core Framework:** [Bootstrap 5](https://getbootstrap.com/)
-   **Scripting:** JavaScript (ES6+), [jQuery](https://jquery.com/)
-   **Styling:** SCSS (Sass), PostCSS
-   **Build Tools:** [Gulp](https://gulpjs.com/), [Webpack](https://webpack.js.org/)
-   **Package Manager:** npm / yarn

## Building and Running
The project uses `gulp` for task automation. Commands should be run from within either the `full-version/` or `starter-kit/` directories, depending on which one you are working on.

### Prerequisites
-   Node.js and npm/yarn installed.

### Setup
1.  Navigate to the desired directory:
    ```bash
    cd full-version
    # OR
    cd starter-kit
    ```
2.  Install dependencies:
    ```bash
    npm install
    # OR
    yarn install
    ```

### Available Scripts
| Command | Description |
| :--- | :--- |
| `npm run serve` | Starts a local development server with BrowserSync (hot reload). |
| `npm run build` | Builds the project for development (outputs to `dist/` or similar). |
| `npm run build:prod` | Builds the project for production (minified assets). |
| `npm run build:js` | Compiles and bundles JavaScript files only. |
| `npm run build:css` | Compiles SCSS files to CSS only. |
| `npm run format:scss` | Fixes SCSS formatting using Stylelint. |

## Development Conventions

### Directory Structure
-   **`html/`**: Contains HTML templates/pages.
-   **`assets/`**: Static assets.
    -   `scss/`: Source SCSS files (Core, Bootstrap overrides, Components).
    -   `js/`: Source JavaScript files.
    -   `img/`, `fonts/`, `vendor/`: Images, fonts, and third-party vendor assets.
-   **`tasks/`**: Gulp task definitions.
-   **`libs/`**: Third-party libraries.

### Code Quality
The project enforces code quality and formatting through configuration files found in the root of each version:
-   **Linting:** ESLint (`.eslintrc.json`) for JavaScript.
-   **Formatting:** Prettier (`.prettierrc.json`).
-   **Styles:** Stylelint (`.stylelintrc.json`) for SCSS.

### Customization
-   **SCSS:** Modify files in `assets/scss/` to customize styles. Avoid editing `libs/` or `vendor/` css directly.
-   **JS:** Application logic resides in `assets/js/`.
-   **Templates:** HTML files are located in `html/`.
