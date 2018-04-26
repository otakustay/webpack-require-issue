Steps to reproduce issue:

1. `npm install`
2. `$(npm bin)/webpack --mode=production src/index.mjs`
3. Open `dist/main.js` and format it
4. Ensure there is a `require("./../node_modules/webpack/buildin/global.js")` call at the end of file

Using `src/index.js` as entry will not produce this issue.
