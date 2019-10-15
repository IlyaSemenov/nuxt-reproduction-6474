Reproduction repo for <https://github.com/nuxt/nuxt.js/issues/6474>.

* Checkout
* Run `yarn`
* Run `yarn test`, it works
* Run `yarn dev`, it crashes:

```
 FATAL  Cannot find module '@/foo'                                                                                                                                       16:43:23
Require stack:
- /Users/semenov/tmp/nuxt/nuxt.config.ts
- /Users/semenov/tmp/nuxt/node_modules/@nuxt/cli/dist/cli-command.js
- /Users/semenov/tmp/nuxt/node_modules/@nuxt/cli/dist/cli.js
- /Users/semenov/tmp/nuxt/node_modules/@nuxt/typescript-runtime/bin/nuxt-ts.js

  Error: Cannot find module '@/foo'
  Require stack:
  - nuxt.config.ts
  - node_modules/@nuxt/cli/dist/cli-command.js
  - node_modules/@nuxt/cli/dist/cli.js
  - node_modules/@nuxt/typescript-runtime/bin/nuxt-ts.js
  at Object.<anonymous> (nuxt.config.ts:3:15)
  at Generator.next (<anonymous>)


   ╭────────────────────────────────────────────────────────────────────────────────────╮
   │                                                                                    │
   │   ✖ Nuxt Fatal Error                                                               │
   │                                                                                    │
   │   Error: Cannot find module '@/foo'                                                │
   │   Require stack:                                                                   │
   │   - /Users/semenov/tmp/nuxt/nuxt.config.ts                                         │
   │   - /Users/semenov/tmp/nuxt/node_modules/@nuxt/cli/dist/cli-command.js             │
   │   - /Users/semenov/tmp/nuxt/node_modules/@nuxt/cli/dist/cli.js                     │
   │   - /Users/semenov/tmp/nuxt/node_modules/@nuxt/typescript-runtime/bin/nuxt-ts.js   │
   │                                                                                    │
   ╰────────────────────────────────────────────────────────────────────────────────────╯
```
