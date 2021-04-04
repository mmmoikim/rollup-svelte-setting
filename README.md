# rollup-svelte-setting

1. npm init
2. npm i svelte
3. npm install -D rollup
4. npm i -D [@rollup/plugin-node-resolve](https://www.npmjs.com/package/@rollup/plugin-node-resolve)

- A Rollup plugin which locates modules using the Node resolution algorithm, for using third party modules in node_modules
- The resulting bundle.js will still work in Node.js, because the import declaration gets turned into a CommonJS require statement, but the-answer does not get included in the bundle. For that, we need a plugin.
- https://rollupjs.org/guide/en/#with-npm-packages

5. npm i -D [@rollup/plugin-commonjs](https://github.com/rollup/plugins/tree/master/packages/commonjs)

- Some libraries expose ES modules that you can import as-is — the-answer is one such module. But at the moment, the majority of packages on NPM are exposed as CommonJS modules instead. Until that changes, we need to convert CommonJS to ES2015 before Rollup can process them.

6. npm i -D [@rollup/plugin-babel](https://www.npmjs.com/package/@rollup/plugin-babel)

- A Rollup plugin for seamless integration between Rollup and Babel.
- Many developers use Babel in their projects in order to use the latest JavaScript features that aren't yet supported by browsers and Node.js.

7. npm i -D [rollup-plugin-svelte](https://github.com/sveltejs/rollup-plugin-svelte)

- Compile Svelte components.

8. npm i -D [rollup-plugin-livereload](https://www.npmjs.com/package/rollup-plugin-livereload)

9. npm i -D [rollup-plugin-terser](https://www.npmjs.com/package/rollup-plugin-terser)

10. npm i -D [rollup-plugin-css-only](https://www.npmjs.com/package/rollup-plugin-css-only)

11. npm i -D [sirv-cli](https://www.npmjs.com/package/sirv-cli)

- By default, sirv will only respond to requests that match files in `public`. This is to maximise compatibility with static fileservers, allowing you to deploy your app anywhere.

- Rollup plugin to minify generated es bundle

8. make rollup.config.js file

-

9. make public/index.html

-

reference
https://typeofnan.dev/how-to-set-up-a-svelte-app-with-rollup/
