# Instruction

## Two step npm link
```
cd foo
npm link
cd ../bar
npm link foo
```
```
sham@sham-home:~/work/yarn-compare-npm/npm-link/foo$ npm link
npm WARN foo@0.0.0 No description
npm WARN foo@0.0.0 No repository field.
/usr/local/lib/node_modules/foo -> /home/sham/work/yarn-compare-npm/npm-link/foo
sham@sham-home:~/work/yarn-compare-npm/npm-link/foo$ cd ../bar/
sham@sham-home:~/work/yarn-compare-npm/npm-link/bar$ npm link foo
/home/sham/work/yarn-compare-npm/npm-link/bar/node_modules/foo -> /usr/local/lib/node_modules/foo -> /home/sham/work/yarn-compare-npm/npm-link/foo
sham@sham-home:~/work/yarn-compare-npm/npm-link/bar$ 
```

## One step npm link
```
cd bar
npm link ../foo
```

```
sham@sham-home:~/work/yarn-compare-npm/npm-link/bar$ npm link ../foo
npm WARN foo@0.0.0 No description
npm WARN foo@0.0.0 No repository field.
/usr/local/lib/node_modules/foo -> /home/sham/work/yarn-compare-npm/npm-link/foo
/home/sham/work/yarn-compare-npm/npm-link/bar/node_modules/foo -> /usr/local/lib/node_modules/foo -> /home/sham/work/yarn-compare-npm/npm-link/foo
sham@sham-home:~/work/yarn-compare-npm/npm-link/bar$ 
```