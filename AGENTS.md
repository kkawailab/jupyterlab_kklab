# Repository Guidelines

## Project Structure & Module Organization

This repository publishes a browser-based JupyterLite site. User-facing notebooks and sample files live under `content/`: top-level notebooks demonstrate the Python, JavaScript, and p5 kernels; `content/pyodide/` contains Pyodide examples; and `content/data/` holds datasets and images used by those notebooks. `repl/jupyter-lite.json` configures the JupyterLite front end. Python and JupyterLab dependencies are pinned in `requirements.txt`, while `.github/workflows/deploy.yml` defines the GitHub Pages build and deployment. The generated `dist/` directory is ignored and must not be committed.

## Build, Test, and Development Commands

Use Python 3.11 to match CI:

```bash
python -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
cp README.md content/
jupyter lite build --contents content --output-dir dist
python -m http.server 8000 --directory dist
```

The first three commands create the environment used by the project. The JupyterLite command performs the production build; the final command serves it at `http://localhost:8000` for browser testing. Remove the copied `content/README.md` after local validation if it is not intended as repository content.

## Coding Style & Naming Conventions

Keep notebooks focused, runnable from top to bottom, and free of incidental output or large embedded data unless the output is part of the demonstration. Prefer descriptive lowercase filenames, using hyphens for multiword examples (for example, `interactive-widgets.ipynb`), while preserving established names in `pyb2d/`. Format Python cells with four-space indentation and standard PEP 8 conventions. Keep JSON valid, consistently indented, and limited to settings required by the site.

## Testing Guidelines

There is no dedicated unit-test suite or coverage threshold. Treat a clean JupyterLite build as the baseline check. Open the generated site in a supported modern Firefox or Chromium browser, launch each changed notebook, restart its kernel, and run all cells. Confirm that widgets, plots, and referenced files load without console or cell errors.

## Commit & Pull Request Guidelines

History currently contains only an `Initial commit`, so no detailed convention is established. Use short, imperative subjects such as `Add Plotly notebook example`. Keep dependency, configuration, and content changes logically separated. Pull requests should explain the user-visible change, list local validation performed, link relevant issues, and include screenshots or recordings for interface, rendering, or visualization changes. Ensure the GitHub Pages build passes before requesting review.

## Dependency & Configuration Notes

Keep compatible version bounds in `requirements.txt`; explain upgrades that alter kernels or rendered output. Never commit credentials, local virtual environments, generated build artifacts, or notebook checkpoints.
