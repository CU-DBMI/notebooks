# CU-DBMI Notebooks

Demonstrational and shareable Jupyter notebooks deployed using JupyterLite on Github Pages.

## Development

Development and deployment of this repo is assisted using Python [Poetry](https://python-poetry.org/docs/) as an environment and package dependency manager. Please ensure Poetry is installed in order to develop content related to this repo.

To create or modify Jupyter notebooks within this repo, use Jupyter via the Poetry configuration. For example

```shell
# only required if the environment has not yet been installed
poetry install
# run jupyter lab, usually resulting in a browser window popping open
poetry run jupyter lab
```

To test your output to ensure it works with JupyterLite, reference the following example:

```shell
# only required if the environment has not yet been installed
poetry install
# build the JupyterLite content to be served
poetry run jupyter lite build --contents content
# run JupyterLite, reference the URL provided from the terminal to view the contents
poetry run jupyter lite serve
```

## References

### JupyterLite

- How-to Guides: <https://jupyterlite.readthedocs.io/en/latest/howto/index.html>
- Reference: <https://jupyterlite.readthedocs.io/en/latest/reference/index.html>
