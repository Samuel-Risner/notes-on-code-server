# Extensions

- For running: `formulahendry.code-runner`
- For linting: `ms-pyright.pyright`

You need to change the execution map for `formulahendry.code-runner` in `.vscode/settings.json`:

## formulahendry.code-runner

You need to either change the execution map for in `.vscode/settings.json`:

```jsonc
{
  "code-runner.executorMap": {
    "python": "python3.11 -u",
  }
}
```

Or use a shebang:

```py
#!/usr/bin/python3.11
```

## ms-pyright.pyright

See here for documentation on configuration: https://github.com/microsoft/pyright/blob/main/docs/configuration.md

# Dockerfile

If everything worked the following commands should run:

```shell
python3.11 --version
```

Output: `Python 3.11.5 (or newer)

```shell
python3.11 -m pip -V
```

Output: `pip 22.0.2 from /usr/lib/python3/dist-packages/pip (python 3.11)` (or newer)

# How to create a virtual environment

```shell
python3.11 -m venv venv
```

# How to install `requirements.txt` with pip

```shell
python3.11 -m pip install -r requirements.txt
```

