# Getting Started

Welcome to MkDocs! MkDocs is a simple and lightweight static site generator, great for project documentation or blogs. MkDocs is built off of your basic markdown file and while this adds to the simplicity, it does come with some draw backs as it is restricted to just the functionalities that an md has. For example, unlike a Quarto document, we will not be able to render graphics just by adding R code blocks, instead we will need to render it beforehand and then add it to the repository.

> If the limitations of a markdown file doesn't work for your project, MkDocs is likely not the best option.
 
For full documentation visit [mkdocs.org](https://www.mkdocs.org).

## Installation

To install MkDocs, run the following command:

```
pip install mkdocs-material
```

## Set Up Project

To begin your new project you can first run the following command:

```
mkdocs new [project name]
```

Then run the following command:

```
cd [project name]
```

Optionally, if you would like to build the blog out of the existing directory, instead run the following command:

```
mkdocs new .
```

## Run Your Website

MkDocs comes with a built-in dev-server that lets you preview your documentation as you work on it. To use this, first make sure that you are in your projects directory, then run the following command:

```
mkdocs serve
```

You can then acess your website by opening [http://127.0.0.1:8000/](http://127.0.0.1:8000/) in your browser.