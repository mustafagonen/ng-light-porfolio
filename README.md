
**My-Portfolio — Personal Portfolio**

Overview
- **Purpose:** Personal portfolio website for showcasing projects, contact information and a short introduction.
- **Tech stack:** Angular, TypeScript, SCSS.

Features
- **Homepage:** Hero section and project highlights.
- **Projects:** Project listing and project detail pages.
- **Contact:** Contact form to allow visitors to get in touch.

Tech Stack
- **Framework:** `Angular`
- **Languages:** `TypeScript`, `SCSS`, `HTML`

Quick Start (Development)
1. Clone the repository:

```
git clone https://github.com/mustafagonen/my-portfolio.git
cd my-portfolio
```

2. Install dependencies:

```
npm install
```

3. Start the development server (PowerShell / Windows):

```
npm start
```

The app will run by default at `http://localhost:4200` (Angular default).

npm scripts
- `npm start`: Runs the development server.
- `npm build` / `npm run build`: Builds the app for production (output goes to `dist/mg-portfolio`).
- `npm test`: Runs unit tests (if configured).

Project Structure (high level)
- `src/`: Application source code.
- `src/app/`: Components, services, pipes and routing.
- `src/assets/`: Images and documents (`images/`, `documents/`).
- `environments/`: `environment.ts` and `environment.prod.ts` (API URLs and environment config).
- `angular.json`, `package.json`: Project configuration and scripts.

Notable files
- `src/app/app.routes.ts` — Application route definitions.
- `src/app/services/` — Services that communicate with backend APIs.
- `src/app/interceptors/` — HTTP interceptors and error handling.

Environment / API notes
- API URLs and environment-specific settings are stored in `src/environments`. Update `environment.ts` or `environment.prod.ts` as needed before building.

Deploying to Netlify
- A `netlify.toml` file is included in the repository to enable seamless deployment from GitHub to Netlify.

Automatic (recommended):
1. Push your repository to GitHub (if it isn't already).
2. On Netlify, choose "New site from Git" → connect your GitHub account and select this repository.
3. Netlify will use the `netlify.toml` settings (build command and publish directory) automatically. The build command used is:

```
npm run build
```

and the publish directory is:

```
dist/mg-portfolio
```

4. Netlify also uses a redirect rule so client-side routes will serve `index.html`.

Manual (if you prefer):
- Build command: `npm run build`
- Publish directory: `dist/mg-portfolio`
- Add any required environment variables (for example `API_URL`) under site settings.

Notes
- The project uses the local Angular CLI from `devDependencies`, so Netlify's build will use the project-installed CLI when running `npm run build`.
- If you need a specific Node.js version, add an `engines` field to `package.json` or set the Node version in Netlify site settings.

Development notes
- When adding new components, import them into the appropriate module (for example `shared.module.ts`) where needed.
- Global styles are managed in `src/styles.scss`.

Contributing
- Fork → create a branch → make changes → open a Pull Request. Use descriptive commit messages and include screenshots or demo links if relevant.

License
- If you want this repository to have an explicit open-source license, add a `LICENSE` file (e.g. `MIT` or `Apache-2.0`).

Contact
- Repository owner: `mustafagonen` (GitHub). If you'd like me to add an email or social link, tell me and I'll update the README.

---

If you'd like additional details (screenshots, live demo link, or a specific license added), tell me and I will update the README accordingly.
# mg-portfolio

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 17.1.3.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page.
