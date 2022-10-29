# AngularPixijsIssue8794

Reproduction steps from this repository:

```sh
git clone git@github.com:Julien-Marcou/angular-pixijs-issue-8794.git
cd angular-pixijs-issue-8794
npm install
ng serve
```


Reproduction steps from a new Angular projects :

```sh
ng new angular-pixijs-issue-8794 --strict --skip-tests --skip-git --minimal --routing --style=scss --inline-style=false --inline-template=false
cd angular-pixijs-issue-8794
npm install pixi.js
# add "import * as PIXI from 'pixi.js';" to the src/main.ts file
# add "allowSyntheticDefaultImports: true" to the tsconfig.json
# add "offscreencanvas" to the tsconfig.app.json's types
ng serve
```
