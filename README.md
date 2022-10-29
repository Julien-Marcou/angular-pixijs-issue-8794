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
# open the file src/main.ts and import pixi.js
ng serve
```
