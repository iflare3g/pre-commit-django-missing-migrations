[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)


pre-commit-django-missing-migrations
================

pre-commit hook to check Django missing model's changes not reflected in migration files.
It will be triggered only when you change a python file called `models` or a file inside a `package` called `models`.
It can be easily used inside a CI, all the instructions can be found inside pre-commit documentation and run it over all files.

### Using this hook with pre-commit

Add this to your `.pre-commit-config.yaml`

```yaml
-   repo: https://github.com/iflare3g/pre-commit-django-missing-migrations/
    rev: 1.0.0
    hooks:
        - id: check-missing-migrations
```
