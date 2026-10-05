<!-- tyhp-readme:start -->
# tyhpdef/giggsey-locale

Tyhp type definitions for `giggsey/locale` `2.9.0`.

```bash
composer require --dev tyhpdef/giggsey-locale:2.9.0
```

This is a metapackage. Composer also installs `tyhpdef/giggsey-locale-impl` (type files).
Require **this** name, not `tyhpdef/giggsey-locale-impl`.

See https://tyhplang.com.

## Maintain `giggsey/locale`? Ship the types yourself

If you are a Packagist maintainer of `giggsey/locale`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/giggsey-locale-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `giggsey/locale` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/giggsey-locale": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `giggsey/locale` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `giggsey/locale` with a real constraint,
   `"replace": { "tyhpdef/giggsey-locale": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `giggsey/locale` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/giggsey-locale` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
