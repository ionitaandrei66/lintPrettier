Linter/prittier/husky

lint-staged este un instrument care te ajută să rulezi automat comenzi (ex: ESLint, Prettier) doar pe fișierele modificate (staged)



Husky este o unealtă care îți permite să rulezi scripturi automat la anumite acțiuni Git (numite git hooks), cum ar fi:
* înainte de commit → (pre-commit)
* înainte de push → (pre-push)
* după merge, checkout, etc.


Pentru ce se folosește?
Husky te ajută să:
* Rulezi automat Prettier și ESLint la fiecare commit.
* Blochezi commit-uri dacă nu trec testele.
* Rulezi teste automat la pre-push.
* Verifici convenții de commit (commitlint, de exemplu).



Prettier este un formatter automat de cod – el rearanjează codul tău automat ca să respecte un stil clar și consistent, indiferent de cine scrie codul
Pentru Prettier ai 2 file după instalare, ai .prettierrc, unde setezi regulile de scriere precum ex mai jos, și .prettierignore
{
  "tabWidth": 2,
  "useTabs": false,
  "semi": true,
  "singleQuote": true,
  "quoteProps": "as-needed",
  "trailingComma": "none",
  "bracketSpacing": true,
  "arrowParens": "always",
  "endOfLine": "auto",
  "printWidth": 120,
  "overrides": [
    {
      "files": "*.html",
      "options": {
        "parser": "angular"
      }
    }
  ]
}



ESLint este un linter – adică un instrument care verifică codul tău pentru erori, probleme de stil și potențiale buguri.


Install and configure ESLint
ng add @angular-eslint/schematics


Install and configure Prettier
npm install prettier --save-dev

Configure Prettier to be used as an ESLint plugin
npm install prettier-eslint eslint-config-prettier eslint-plugin-prettier



# LintPrettier

This project was generated using [Angular CLI](https://github.com/angular/angular-cli) version 19.2.3.

## Development server

To start a local development server, run:

```bash
ng serve
```

Once the server is running, open your browser and navigate to `http://localhost:4200/`. The application will automatically reload whenever you modify any of the source files.

## Code scaffolding

Angular CLI includes powerful code scaffolding tools. To generate a new component, run:

```bash
ng generate component component-name
```

For a complete list of available schematics (such as `components`, `directives`, or `pipes`), run:

```bash
ng generate --help
```

## Building

To build the project run:

```bash
ng build
```

This will compile your project and store the build artifacts in the `dist/` directory. By default, the production build optimizes your application for performance and speed.

## Running unit tests

To execute unit tests with the [Karma](https://karma-runner.github.io) test runner, use the following command:

```bash
ng test
```

## Running end-to-end tests

For end-to-end (e2e) testing, run:

```bash
ng e2e
```

Angular CLI does not come with an end-to-end testing framework by default. You can choose one that suits your needs.

## Additional Resources

For more information on using the Angular CLI, including detailed command references, visit the [Angular CLI Overview and Command Reference](https://angular.dev/tools/cli) page.
