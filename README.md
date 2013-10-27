# WordPress Sublime Text 2

Autocomplete for WordPress Functions, Hooks, Constants, Classes.
Also some Snippets for WordPress Boilerplate.

### Features

Autocomplete for:

    WP version : 3.7.0

    Functions          : 1734
    Hooks              : 1434
    Constants/Classes  :  191

Deprecated functions (219) have been removed :smiley_cat:

This version also adds the ability for the first "tab" to delete ALL parameters instead of having to tab through each one, which is super useful:

- First Tab-->Select all parameters
- Each Tab Thereafter-->Selects each individual parameter or block

### Snippets

Snippets are slowly being added, to call a snippet you use the same function name, the autocomplete will show an "ALL Options" selection. For example to
register a custom post type you would write `register_post...`

Current Snippets:

 - `plugin` : Creates plugin boilerplate
 - `WP_Query` : Creates new WP_Query class
 - `wp_enqueue` : Creates wp_enqueue function
 - `register_post_type` : Register Post Type All Options
 - `register_sidebar`  : Register Taxonomy All Options
 - `register_taxonomy`  : Register Taxonomy All Options
 - `wp_nav_menu` : wp_nav_menu All Options

### Tip

Sublime won't autocomplete PHP files when there is no closing `?>` tags , so in "Preferences-->Settings-User" add this snippet:

    "auto_complete_selector": "source, text",

### Notes

The other WordPress sublime package was not up to date, missing some features and stuff, so I build a [custom parser](https://github.com/wycks/WP-Hooks/tree/gh-pages/Sublime-Parser) for grabbing data from WP core.

Some hooks/functions have duplicated names throughout the WP code-base, so it is necessarily to tab through the options for some autocompletes, typically the function(s) are first followed by the hooks.

Hooks names which start as a variable have been removed, for example `do_action($page_hook)`, there are not many in WP and there is no great way to add them to Sublime.

### ToDo

Add more snippets

#### Manual

Download the .zip or git clone this into your sublime packages location, you can find it under "Preferences-->Browse Packages".

