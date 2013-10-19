# SCSS folder styleguide

This is a basic folder structure to quickstart a yet undefined project.

## Folder Structure

This structure is aiming for that you would be able to create a websites just with your /global files.
Like a framework. Here you declare all the basic elements that the project needs.
Everything else would be an "extensions" and so defined within a module.
Therefore it's important to keep the loading order in main.scss.

### Fonts

Load in all @font-face that you use within your project.
If you prefer to use external resources you may delete this file.
It's loaded at first to make sure you can access your fonts with variables.

### Variables

Here you declare all variables that will be used within your project.
If there are module specific varibles, put them right into your module file.

### Functions

Here you declare all your function that will be used within your project.
If there's a function that is module specific, put your function within your module file.

### Mixins

Here you declare all your mixins that will be used within your project.
If there's a mixin that is module specific, put your function within your module file.

### Typography

Here you declare all your layout specifiy typography that will be the base of your project.
Module specific typography will be declared in your module file.

### Layout

Here you declare all your layout specifiy styles that will be the base of your project.
Everything else is a module.

## Modules

Everything that is not a global style defined in _layout.scss is a module.

## Vendor

If you use plugins that have a specific style file put them here to use them within your module.
Make sure to reference a vendor file within your module if you use it.

