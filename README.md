# Angular PixiJS Issue #8794

See https://github.com/pixijs/pixijs/issues/8794

Reproduction steps from this repository:

```sh
git clone git@github.com:Julien-Marcou/angular-pixijs-issue-8794.git
cd angular-pixijs-issue-8794
npm install
ng serve
```

Reproduction steps for a new Angular project:

```sh
ng new angular-pixijs-issue-8794 --strict --skip-tests --skip-git --minimal --routing --style=scss --inline-style=false --inline-template=false
cd angular-pixijs-issue-8794
npm install pixi.js
# add "import * as PIXI from 'pixi.js';" to the src/main.ts file
# add "allowSyntheticDefaultImports: true" to the tsconfig.json
# add "offscreencanvas" to the tsconfig.app.json's types
ng serve
```

Build logs:

```sh
Error: node_modules/@pixi/events/lib/FederatedEventTarget.d.ts:11:18 - error TS2320: Interface 'FederatedEventTarget' cannot simultaneously extend types 'EventEmitter<string | symbol, any>' and 'EventTarget'.
  Named property 'removeAllListeners' of types 'EventEmitter<string | symbol, any>' and 'EventTarget' are not identical.

11 export interface FederatedEventTarget extends utils.EventEmitter, EventTarget {
                    ~~~~~~~~~~~~~~~~~~~~
```