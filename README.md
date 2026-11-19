# Maho NAME

![Maho Commerce](https://img.shields.io/badge/Maho_Commerce-module-orange)
![License](https://img.shields.io/badge/license-OSL--3.0-blue)
![PHP](https://img.shields.io/badge/php-%3E%3D8.5-8892BF)
![PHPStan Level](https://img.shields.io/badge/PHPStan-level%208-brightgreen)

**TODO: one-line pitch.** Longer description of what this module does, who it's for, and the integration it provides for [Maho Commerce](https://mahocommerce.com).

## Requirements

- PHP >= 8.5
- Maho Commerce

## Installation

```bash
composer require mahocommerce/module-name
```

## Configuration

TODO: how to enable and configure the module from the Maho admin (System → Configuration → ...).

## Development

This module ships with the standard Maho CI gates:

- **PHPStan** (level 8) — `vendor/bin/phpstan analyze`
- **Rector** (dry-run) — `vendor/bin/rector --dry-run`
- **PHP CS Fixer** (dry-run) — `vendor/bin/php-cs-fixer fix --dry-run`
- **PHP / XML syntax checks** — automatic on CI

Run `composer install` and you can execute any of the above locally before pushing. Composer prefers stable releases and can install beta dependencies when Maho requires them. PHPStan runs once there are PHP or PHTML files under `app/`.

---

## Using this template

When you create a new repo from this template:

1. **Rename placeholders** in the new repository.
   - Replace `mahocommerce/module-name` in `composer.json` and the install command with your lowercase Composer package name.
   - Replace `module-NAME` in `.github/SECURITY.md` with the GitHub repository name.
   - Replace `NAME` in the title and write the module description in `composer.json` and `README.md`.
2. **Update the badge URLs** if you want CI status badges (they're not included by default — the 4 static badges above are the org standard).
3. **Bootstrap the module code** under `app/code/community/Vendor/Module/` (or `app/code/core/Maho/Module/` for first-party Maho modules) and declare it in `app/etc/modules/Vendor_Module.xml`.
4. **Add `.github/FUNDING.yml`** (already included — leave as-is for org-owned repos, edit/remove for forks).
5. **Update this section** of the README with the real module docs once you've shipped something.

See an existing module for reference: [module-mollie](https://github.com/MahoCommerce/module-mollie), [module-przelewy24](https://github.com/MahoCommerce/module-przelewy24).
