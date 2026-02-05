# Readme

Personal website built with [Quarto](https://quarto.org) and hosted on [Github Pages](https://docs.github.com/en/pages).

## Virtual environments

### Python

Using `venv` on Mac OS (see [Quarto documentation](https://quarto.org/docs/projects/virtual-environments.html#using-venv))

#### Use the environment

*In the Terminal*

Go inside the project's folder and:

```zsh
source env/bin/activate
```

*Interactive Python*

Nothing to do. VS Code should pick up the environment automatically.

#### Install a new package

*Terminal*

```zsh
python3 -m pip install {package name}
```

*Interactive Python*

```python
pip install {package name}
```

#### Save the environment

*Terminal*

```zsh
python3 -m pip freeze > requirements.txt
```

*Interactive Python*

```python
pip freeze > requirements.txt
```

### R

#### Check status

In the project's folder, open an R terminal :

```r
renv::status()
```

#### Install new package

```r
renv::install("{package name}")
```

#### Save environment

```r
renv::snapshot(lockfile = "renv.lock")
```
