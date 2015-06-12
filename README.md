# Invo Recipes

## Recipes
To add a new recipe, create a new mardown file in the `_recipes` directory. You should place it in the appropriate folder, but also make sure you specify the category in the frontmatter. For instance, the following mardown file would be placed in `_recipes/main/little_boys.md`.

```
---
layout: recipe
title: Little Boys
author: jsonin
category: main
yield: 1 child
---

* Snips
* Snails
* Puppy-dog tails

Mix all ingredients, careful to not mince the puppy dog tails.

```
When the site is built, this will generate `/recipes/main/little_boys.index`. Note that the url generated is based on the directory the recipe is placed in. The listing on the main page is generated based on the `category` field.

## Authors
The metadata about the authors are stored in `_data/authors.json`. In order to add a new author, simply add a new item in the object. The key of the object should match what is shown in the `author` field of the markdown front matter in the recipe.

## Categories
To add a new category (say `lunch`), add the appropriate directory in the recipes directory (`_recipes\lunch`) and make a new file named `_recipes/lunch.html`. Make the properties match the existing examples.

## License

Open sourced under the [MIT license](LICENSE.md).

<3
