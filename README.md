# Artifactual Intelligence


## Abstract

Artificial intelligence has seen a resurgence in the public’s attention
thanks to innovations in large language models (LLMs). While every
technological innovation comes with its own well-studied lifecycle from
hype to normalcy, LLMs particular flavor of *narrow* artificial
intelligence seems different. To an extent that may well be unique among
technologies, today’s artificial intelligence is not understood – even
by those who create it. In this paper we provide a perspective on
artificial intelligence rooted in the history of humanity’s efforts to
understand the world around them, from economic calculation to
probabilistic machine learning. This perspective allows us to see what
AI really is – not artifical, but *artifactual* – and how it might
enable an epistemological revolution.

## Project Organization

- `/code` Scripts with prefixes (e.g., `01_import-data.py`,
  `02_clean-data.py`) and functions in `/code/src`.
- `/data` Simulated and real data, the latter not pushed.
- `/figures` PNG images and plots.
- `/output` Output from model runs, not pushed.
- `/presentations` Presentation slides.
- `/private` A catch-all folder for miscellaneous files, not pushed.
- `/renv` Project library, once initialized (see below).
- `/writing` Case studies and the paper.
- `/.venv` Hidden project library, not pushed.
- `.gitignore` Hidden Git instructions file.
- `.python-version` Hidden Python version for the reproducible
  environment.
- `renv.lock` Information on the reproducible environment.
- `requirements.txt` Information on the reproducible environment.

## Reproducible Environment

### Python

After cloning this repository, go to the project’s terminal in Positron
and run `python -m venv .venv` to create the `/.venv` project library,
followed by `pip install -r requirements.txt` to install the specified
library versions.

Whenever you install new libraries or decide to update the versions of
libraries you use, run `pip freeze > requirements.txt` to update
`requirements.txt`.

### R

Add a reproducible environment by creating a project library using the
`{renv}` package.

- Initialize the project library *once* using `renv::init()`.
- Once you’ve installed packages, add them to the project library using
  `renv::snapshot()`.
- If a project library already exists, install the associated packages
  with `renv::restore()`.

For more details on using GitHub, Quarto, etc. see [ASC
Training](https://github.com/marcdotson/asc-training).
