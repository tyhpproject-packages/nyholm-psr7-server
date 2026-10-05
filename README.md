<!-- tyhp-readme:start -->
# tyhpdef/nyholm-psr7-server

Tyhp type definitions for `nyholm/psr7-server` `1.1.0`.

```bash
composer require --dev tyhpdef/nyholm-psr7-server:1.1.0
```

This is a metapackage. Composer also installs `tyhpdef/nyholm-psr7-server-impl` (type files).
Require **this** name, not `tyhpdef/nyholm-psr7-server-impl`.

See https://tyhplang.com.

## Maintain `nyholm/psr7-server`? Ship the types yourself

If you are a Packagist maintainer of `nyholm/psr7-server`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/nyholm-psr7-server-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `nyholm/psr7-server` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/nyholm-psr7-server": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `nyholm/psr7-server` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `nyholm/psr7-server` with a real constraint,
   `"replace": { "tyhpdef/nyholm-psr7-server": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `nyholm/psr7-server` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/nyholm-psr7-server` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
