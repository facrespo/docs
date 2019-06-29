# OpenML documentation

## Documentation structure
The OpenML documentation in written in MarkDown. The sources are generated by [MkDocs](http://www.mkdocs.org/), using the [Material theme](https://squidfunk.github.io/mkdocs-material/). Check these links to see what is possible in terms of styling.

The overal structure (navigation) of the docs is configurated in the `mkdocs.yml` file.

Some of the API's use other documentation generators, such as Sfinx in openml-python. This documentation is pulled in via iframes to gather all docs into the same place, but they need to be edited in their own GitHub repo's. 

## Editing documentation
Documentation can be edited by simply editing the markdown files in the `docs` folder and creating a pull request.

End users can edit the docs by simply clicking the edit button (the pencil icon) on the top of every documentation page. It will open up an editing page on [GitHub](https://github.com/) (you do need to be logged in on GitHub). When you are done, add a small message explaining the change and click 'commit changes'. On the next page, just launch the pull request. We will then review it and approve the changes, or discuss them if necessary. 

## Deployment
The documentation is hosted on GitHub pages.

To deploy the documentation, you need to have MkDocs and MkDocs-Material installed, and then run `mkdocs gh-deploy` in the top directory (with the `mkdocs.yml` file). This will build the HTML files and push them to the gh-pages branch of openml/docs. `https://docs.openml.org` is just a reverse proxy for `https://openml.github.io/docs/`.  

MKDocs and MkDocs-Material can be installed as follows:
```
pip install mkdocs
pip install mkdocs-material
pip install -U fontawesome_markdown
```

