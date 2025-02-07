# Markdown Theme for phpDocumentor

This repository provides a **Markdown theme for [phpDocumentor](https://www.phpdoc.org/)** that generates API documentation in Markdown format. It also creates a `navigation.yaml` file, making it easy to integrate the generated documentation into [MkDocs](https://www.mkdocs.org/) and then into **Backstage** or other documentation platforms.

---

## Features

- **Markdown-based Output**: Generates API documentation as Markdown files.
- **`navigation.yaml` Generation**: Automatically creates a `navigation.yaml` file for use with MkDocs.
- **Backstage-Friendly**: The Markdown structure and navigation file integrate seamlessly with Backstage.

---

## Prerequisites

- **phpDocumentor**: [Installation guide](https://docs.phpdoc.org/3.0/guide/getting-started/installing.html)
- **Theme Extension**: [phpdoc-backstage-markdown-extension](https://github.com/axelerant/phpdoc-backstage-markdown-extension)

---

## Installation

1. **Clone or download** this repository to a location accessible by your project.
2. Copy the `markdown-theme` folder to your projects `.phpdoc/themes` directory, or a location of your choosing.
3. Copy the `phpdoc-backstage-markdown-extension` folder to your projects `.phpdoc/extesions` directory.
4. Generate the docs using docker
    ```bash
    docker run --rm -v "$(pwd):/data" "phpdoc/phpdoc:3-unstable" --template=".phpdoc/themes/phpdoc-backstage-markdown-theme"
    ```
