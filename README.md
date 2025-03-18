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
