# SCSS folder styleguide

This is a basic folder structure to quickstart a yet undefined project.

## Folder Structure

This structure is aiming for that you would be able to create a websites just with your /global files.
Like a framework. Here you declare all the basic elements that the project needs.
Everything else would be an "extensions" and so defined within a module.
Therefore it's important to keep the loading order in main.scss.

### Global

#### _fonts.scss

Load in all @font-face that you use within your project.
If you prefer to use external resources you may delete this file.
It's loaded at first to make sure you can access your fonts with variables.

#### _variables.scss

Here you declare all variables that will be used within your project.
If there are module specific varibles, put them right into your module file.

#### _functions.scss

Here you declare all your function that will be used within your project.
If there's a function that is module specific, put your function within your module file.

#### _mixins.scss

Here you declare all your mixins that will be used within your project.
If there's a mixin that is module specific, put your function within your module file.

#### _typography.scss

Here you declare all your layout specifiy typography that will be the base of your project.
Module specific typography will be declared in your module file.

#### _layout.scss

Here you declare all your layout specifiy styles that will be the base of your project.
Everything else is a module.

### Modules

#### _module-name.scss

Everything that is not a global style defined in _layout.scss is a module.

### Vendor

#### _vendor-style.scss

If you use plugins that have a specific style file put them here to use them within your module.
Make sure to reference a vendor file within your module if you use it.

### Comment Style

Make sure you use a straight comment style throughout your project.

The following example is based on https://github.com/necolas/idiomatic-css

```
/* ==========================================================================
   Section comment block
   ========================================================================== */

/* Sub-section comment block
   ========================================================================== */

/**
 * Short description using Doxygen-style comment format
 *
 * The first sentence of the long description starts here and continues on this
 * line for a while finally concluding here at the end of this paragraph.
 *
 * The long description is ideal for more detailed explanations and
 * documentation. It can include example HTML, URLs, or any other information
 * that is deemed necessary or useful.
 *
 * @tag This is a tag named 'tag'
 *
 * TODO: This is a todo statement that describes an atomic task to be completed
 *   at a later date. It wraps after 80 characters and following lines are
 *   indented by 2 spaces.
 */

/* Basic comment */
```

