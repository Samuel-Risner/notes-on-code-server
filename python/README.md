# Extensions

- For running: `formulahendry.code-runner`
- For linting: `ms-pyright.pyright`

You need to change the execution map for `formulahendry.code-runner` in `.vscode/settings.json`:

```jsonc
{
  "code-runner.executorMap": {
    # ...
    "python": "python3.8 -u",
    # ...
  }
}
```

# Dockerfile

If everything worked these commands should run:

```shell
virtualenv --version
# Output: virtualenv 20.13.0+ds from /usr/lib/python3/dist-packages/virtualenv/__init__.py
python3.8 --version
# Output: Python 3.8.18
```
