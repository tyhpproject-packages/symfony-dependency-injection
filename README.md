<!-- tyhp-readme:start -->
# tyhpdef/symfony-dependency-injection

Tyhp type definitions for `symfony/dependency-injection` `7.4.17`.

```bash
composer require --dev tyhpdef/symfony-dependency-injection:7.4.17
```

This is a metapackage. Composer also installs `tyhpdef/symfony-dependency-injection-impl` (type files).
Require **this** name, not `tyhpdef/symfony-dependency-injection-impl`.

See https://tyhplang.com.

## Maintain `symfony/dependency-injection`? Ship the types yourself

If you are a Packagist maintainer of `symfony/dependency-injection`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/symfony-dependency-injection-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `symfony/dependency-injection` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/symfony-dependency-injection": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `symfony/dependency-injection` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `symfony/dependency-injection` with a real constraint,
   `"replace": { "tyhpdef/symfony-dependency-injection": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `symfony/dependency-injection` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/symfony-dependency-injection` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
