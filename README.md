# Open Recipes web site

This is the web site for the Open Recipes project. It uses Flask, Flask-FlatPages, and Frozen-Flask to generate static HTML content.

## Previewing during dev:

    python openrecipes.py

## Building the static site

    # this will output the site into the /build directory
    python openrecipes.py build

## Adding pages

Put a file in the `/pages` directory with a name like `file-name.md` extention. The page will be served as HTML from the path `/file-name/`

## Deploying the site

First, add the main openrecipes repo as a remote:

	git remote add openrecipes-main git@github.com:fictivekin/openrecipes.git

Next, make sure to regen the site:

	python openrecipes.py build

Then we deploy in a way that is currently obscure.