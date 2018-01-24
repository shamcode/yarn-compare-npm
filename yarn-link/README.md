# Instruction

## Two step yarn link
```
cd foo
yarn link
cd ../bar
yarn link foo
```
```
sham@sham-home:~/work/yarn-compare-npm/yarn-link/foo$ yarn link
yarn link v1.3.2
success Registered "foo".
info You can now run `yarn link "foo"` in the projects where you want to use this module and it will be used instead.
Done in 0.15s.
sham@sham-home:~/work/yarn-compare-npm/yarn-link/foo$ cd ../bar/
sham@sham-home:~/work/yarn-compare-npm/yarn-link/bar$ yarn link foo
yarn link v1.3.2
success Using linked module for "foo".
Done in 0.10s.
sham@sham-home:~/work/yarn-compare-npm/yarn-link/bar$ ls -l node_modules/
итого 0
lrwxrwxrwx 1 sham sham 9 янв 24 12:07 foo -> ../../foo
sham@sham-home:~/work/yarn-compare-npm/yarn-link/bar$ 
```
## Unlink
```
cd foo
yarn unlink
```