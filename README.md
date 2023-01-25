# Playing with [Quarto](https://quarto.org/)

## Setup

1. Install Quarto via the [Installer page](https://quarto.org/docs/get-started/)
2. Install an [IDE extension of your choice](https://quarto.org/docs/get-started/)
3. Create a Python virtual environment
  ```bash
  $ python -m venv venv
  $ . venv/bin/activate
  (venv) $ pip install -r requirements.txt
  ```
4. Create .html with `quarto render`
  ```bash
  $ .venv/bin/activate
  (venv) $ quarto render hello.qmd
  ```

## Notes

- For every quarto markdown file `.qmd` it creates a folder `FILENAME_files` that contains assets relating to that html file
  - figure images
  - associated javascript and css
  I've ignored these in .gitignore as if we wanted to serve this on GitHub pages these can be generated through an Action.