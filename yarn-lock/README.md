# Instruction

```
cd foo
yarn
yarn link
cd ../bar
yarn link foo
yarn cache clean
yarn install --offline
```

```
sham@sham-home:~/work/yarn-compare-npm/yarn-lock/bar$ yarn install --offline
yarn install v1.3.2
[1/4] Resolving packages...
error Couldn't find any versions for "foo" that matches "*" in our cache (possible versions are ""). This is usually caused by a missing entry in the lockfile, running Yarn without the --offline flag may help fix this issue.
info Visit https://yarnpkg.com/en/docs/cli/install for documentation about this command.
sham@sham-home:~/work/yarn-compare-npm/yarn-lock/bar$ 
```

## Unlink
```
cd foo
yarn unlink
```