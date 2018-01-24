# Instruction

## Fail npm shrinkwrap with linked packages & devDependencies  
```
mkdir -p bar/node_modules
ln -rsf ./foo/ ./bar/node_modules/foo
cd foo
npm install
npm shrinkwrap
cd ../bar
npm shrinkwrap
```

```
sham@sham-home:~/work/yarn-compare-npm/npm-shrinkwrap/bar$ npm shrinkwrap
npm ERR! Linux 3.16.0-5-amd64
npm ERR! argv "/usr/local/bin/node" "/usr/local/bin/npm" "shrinkwrap"
npm ERR! node v6.9.3
npm ERR! npm  v3.10.10

npm ERR! Problems were encountered
npm ERR! Please correct and try again.
npm ERR! extraneous: @babel/code-frame@7.0.0-beta.31 /home/sham/work/yarn-compare-npm/npm-shrinkwrap/bar/node_modules/foo/node_modules/@babel/code-frame
npm ERR! extraneous: @babel/helper-function-name@7.0.0-beta.31 /home/sham/work/yarn-compare-npm/npm-shrinkwrap/bar/node_modules/foo/node_modules/@babel/helper-function-name
npm ERR! extraneous: @babel/helper-get-function-arity@7.0.0-beta.31 /home/sham/work/yarn-compare-npm/npm-shrinkwrap/bar/node_modules/foo/node_modules/@babel/helper-get-function-arity
npm ERR! extraneous: @babel/template@7.0.0-beta.31 /home/sham/work/yarn-compare-npm/npm-shrinkwrap/bar/node_modules/foo/node_modules/@babel/template
npm ERR! extraneous: @babel/traverse@7.0.0-beta.31 /home/sham/work/yarn-compare-npm/npm-shrinkwrap/bar/node_modules/foo/node_modules/@babel/traverse
npm ERR! extraneous: @babel/types@7.0.0-beta.31 /home/sham/work/yarn-compare-npm/npm-shrinkwrap/bar/node_modules/foo/node_modules/@babel/types
npm ERR! extraneous: ansi-styles@3.2.0 /home/sham/work/yarn-compare-npm/npm-shrinkwrap/bar/node_modules/foo/node_modules/ansi-styles
npm ERR! extraneous: babel-eslint@8.1.1 /home/sham/work/yarn-compare-npm/npm-shrinkwrap/bar/node_modules/foo/node_modules/babel-eslint
npm ERR! extraneous: babylon@7.0.0-beta.31 /home/sham/work/yarn-compare-npm/npm-shrinkwrap/bar/node_modules/foo/node_modules/babylon
npm ERR! extraneous: chalk@2.3.0 /home/sham/work/yarn-compare-npm/npm-shrinkwrap/bar/node_modules/foo/node_modules/chalk
npm ERR! extraneous: color-convert@1.9.1 /home/sham/work/yarn-compare-npm/npm-shrinkwrap/bar/node_modules/foo/node_modules/color-convert
npm ERR! extraneous: color-name@1.1.3 /home/sham/work/yarn-compare-npm/npm-shrinkwrap/bar/node_modules/foo/node_modules/color-name
npm ERR! extraneous: debug@3.1.0 /home/sham/work/yarn-compare-npm/npm-shrinkwrap/bar/node_modules/foo/node_modules/debug
npm ERR! extraneous: escape-string-regexp@1.0.5 /home/sham/work/yarn-compare-npm/npm-shrinkwrap/bar/node_modules/foo/node_modules/escape-string-regexp
npm ERR! extraneous: eslint-scope@3.7.1 /home/sham/work/yarn-compare-npm/npm-shrinkwrap/bar/node_modules/foo/node_modules/eslint-scope
npm ERR! extraneous: eslint-visitor-keys@1.0.0 /home/sham/work/yarn-compare-npm/npm-shrinkwrap/bar/node_modules/foo/node_modules/eslint-visitor-keys
npm ERR! extraneous: esrecurse@4.2.0 /home/sham/work/yarn-compare-npm/npm-shrinkwrap/bar/node_modules/foo/node_modules/esrecurse
npm ERR! extraneous: estraverse@4.2.0 /home/sham/work/yarn-compare-npm/npm-shrinkwrap/bar/node_modules/foo/node_modules/estraverse
npm ERR! extraneous: esutils@2.0.2 /home/sham/work/yarn-compare-npm/npm-shrinkwrap/bar/node_modules/foo/node_modules/esutils
npm ERR! extraneous: globals@10.4.0 /home/sham/work/yarn-compare-npm/npm-shrinkwrap/bar/node_modules/foo/node_modules/globals
npm ERR! extraneous: has-flag@2.0.0 /home/sham/work/yarn-compare-npm/npm-shrinkwrap/bar/node_modules/foo/node_modules/has-flag
npm ERR! extraneous: invariant@2.2.2 /home/sham/work/yarn-compare-npm/npm-shrinkwrap/bar/node_modules/foo/node_modules/invariant
npm ERR! extraneous: js-tokens@3.0.2 /home/sham/work/yarn-compare-npm/npm-shrinkwrap/bar/node_modules/foo/node_modules/js-tokens
npm ERR! extraneous: lodash@4.17.4 /home/sham/work/yarn-compare-npm/npm-shrinkwrap/bar/node_modules/foo/node_modules/lodash
npm ERR! extraneous: loose-envify@1.3.1 /home/sham/work/yarn-compare-npm/npm-shrinkwrap/bar/node_modules/foo/node_modules/loose-envify
npm ERR! extraneous: ms@2.0.0 /home/sham/work/yarn-compare-npm/npm-shrinkwrap/bar/node_modules/foo/node_modules/ms
npm ERR! extraneous: object-assign@4.1.1 /home/sham/work/yarn-compare-npm/npm-shrinkwrap/bar/node_modules/foo/node_modules/object-assign
npm ERR! extraneous: supports-color@4.5.0 /home/sham/work/yarn-compare-npm/npm-shrinkwrap/bar/node_modules/foo/node_modules/supports-color
npm ERR! extraneous: to-fast-properties@2.0.0 /home/sham/work/yarn-compare-npm/npm-shrinkwrap/bar/node_modules/foo/node_modules/to-fast-properties
npm ERR! 
npm ERR! If you need help, you may report this error at:
npm ERR!     <https://github.com/npm/npm/issues>

npm ERR! Please include the following file with any support request:
npm ERR!     /home/sham/work/yarn-compare-npm/npm-shrinkwrap/bar/npm-debug.log
sham@sham-home:~/work/yarn-compare-npm/npm-shrinkwrap/bar$ 
```
