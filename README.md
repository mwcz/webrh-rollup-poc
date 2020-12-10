Example of using rollup to generate a bundle of specific Patternfly Elements.

Steps:

 1. in webrh, npm install the desired components (already done, I'm pretty sure!)
 1. npm install `rollup` and `@rollup/plugin-node-resolve`
 1. Create a js file that imports those components, index.js in this example.  All it needs to do is import them, nothing else.
 1. Create rollup.config.js like the one in this exmaple, that specifies the input file (index.js) and output file (bundle.js) and output file format (iife, umd would also work).  It should also import and register the node-resolve plugin
 1. run `rollup -c` (aliased to `npm run build` in this example)
