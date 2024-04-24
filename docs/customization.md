# Customization

Most of the customization that occurs within MkDocs is done in the mkdocs.yml. We will go over a few of the basic things that can be done in MkDocs and Material for MkDocs, then go over how the differences of customization between the two. Having strong knowledge about the functionality of markdown documents will help customize the pages themselves. For example, page table of contents are dictated by the header table of contents. If you would like to include code, you would use the standard markdown code blocks which render on the website as follows:

```{python}
import plotly.express as px

print('Hello World')

x = 3 + 5
```

If you would like to highlight your code as it would appear in a normal file, there is some more complex steps that I will not cover here, but it would appear as follows:

```py
import plotly.express as px

print('Hello World')

x = 3 + 5
```

## Site Name

Changing the site name is a rather easy task, in the mkdocs.yml you would use the following code:

```
site_name: [My Site Name]
```

## Navigation Bar

As mentioned, MkDocs already automatically renders a "table of contents" or "nav bar" for a page based off of the header sizes, but what if you would like to include more pages? First go into the docs folder and add a new markdown file, lets call it "about.md". Now in the mkdocs.yml, to include a nav bar to both markdown pages use the following code:

```
nav:
  - Home: index.md
  - About: about.md
```

There is also the option to split a tab on the nav bar into further pages, lets say you would like to split the about tab into two pages "Getting Started" and "How To" for the markdown files "start.md" and "how.md". In the mkdocs.yml you would then use the following code:

```
nav:
  - Home: index.md
  - 'About':
    - 'Getting Started': 'start.md'
    - 'How To': 'how.md'
```

## Theme

This is where we introduce the main seperation of base MkDocs and Material for MkDocs. MkDocs comes with very few base themes, some of those being the default and 'readthedocs'. Default theme requires no changes, but to use 'readthedocs', in mkdocs.yml use the following code:

```
theme: readthedocs
```

While base MkDocs is slick for a simple site, it doesn't offer the most features. This is where Material for MkDocs comes in. Material for MkDocs provides a new theme that allows for easy adjustment of features, colors, extensions, etc. In order to implement it, in the MkDocs.yml use the following code:

```
theme:
  name: material
```

This allows access to the plethora of options in this package. 

> It is important to note that all sites built on Material for MkDocs will have the same overall structure. Custom themes will require knowledge of HTML or CSS and will be built upon base MkDocs.

## Next Steps

I have so far covered very basic information on what can be done with MkDocs and Material for MkDocs. To learn more about how to use these website frameworks, please refer to the following sites:

* [https://www.mkdocs.org/](https://www.mkdocs.org/)
* [https://squidfunk.github.io/mkdocs-material/](https://squidfunk.github.io/mkdocs-material/)

