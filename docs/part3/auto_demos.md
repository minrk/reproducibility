# Jupytext
As shown in [Publishing a Jupyter book](publishing), we can add `.ipynb` files to the Jupyter book. This is achieved by adding their relative path with respect to `index.md` to `_toc.yml`.

These files can either be generated by hand, and added to the `docs` or auto-generated from a `.py` file, using `jupytext`.

The command
```bash
jupytext --to=ipynb --set-kernel=python3 path/to/demo.py --output=path/to/docs.ipynb
```
generates a notebook compatible with *Jupyter Book*.

The Python file should follow the conventions of the [light format](https://jupytext.readthedocs.io/en/latest/formats.html#the-light-format) for appropriate rendering.

This is illustrated in the following auto-converted demo.

## Auto-conversion of demos

In the [Makefile](https://github.com/jorgensd/reproducibility/blob/main/Makefile) one can find the instructions for auto-converting the demos and building the book.
