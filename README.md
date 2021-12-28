this is a repro repository for a parcel bug regarding relative path containing "`..`"

to reproduce:
```sh
cd library
yarn
yarn dev # this works ✅
```

then:
```sh
cd front
yarn
yarn dev:front # this works ✅
yarn dev:library # this doesn't work ⛔
yarn dev # this doesn't work either ⛔

```
