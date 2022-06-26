# Steps to reproduce

```sh
# Install
yarn

# Run tsx (repl)
yarn tsx
```

The following error appears:
```
node:fs:1551
  handleErrorFromBinding(ctx);
  ^

Error: ENOTDIR: not a directory, stat '/Users/amitda/dev/tmp-tsx/.yarn/cache/tsx-npm-3.6.0-6604a23e18-36fe6fccba.zip/node_modules/tsx/dist/loader.js'
    at statSync (node:fs:1551:3)
    at tryStatSync (node:internal/modules/esm/resolve:189:13)
    at finalizeResolution (node:internal/modules/esm/resolve:430:17)
    at moduleResolve (node:internal/modules/esm/resolve:1009:10)
    at defaultResolve (node:internal/modules/esm/resolve:1218:11)
    at ESMLoader.resolve (node:internal/modules/esm/loader:580:30)
    at ESMLoader.getModuleJob (node:internal/modules/esm/loader:294:18)
    at ESMLoader.import (node:internal/modules/esm/loader:380:22)
    at initializeLoader (node:internal/process/esm_loader:74:49)
    at loadESM (node:internal/process/esm_loader:87:11) {
  errno: -20,
  syscall: 'stat',
  code: 'ENOTDIR',
  path: '/Users/amitda/dev/tmp-tsx/.yarn/cache/tsx-npm-3.6.0-6604a23e18-36fe6fccba.zip/node_modules/tsx/dist/loader.js'
}
```