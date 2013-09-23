# WordPress Sublime Text 2

Autocomplete for WordPress Functions, Hooks, Constants, Classes, and Snippets for WordPress Biolerplate  / Sublime Text 2

### Notes

The other WordPress sublime package was not up to date, missing some features and stuff, so I build a custom parser for grabbing data from WP core.

Also adds the ability for the first "tab" to delete the parameters instead of autocompletintg them which is super useful:

- First Tab-->Select all parameters
- Each Tab Thereafter-->Selects each individual parameter

Deprecated functions (218) have been removed :smiley_cat: 

    Current WP version : 3.6.1
     
    Functions  : 1712
    Hooks      : 1446
    Constants  :  188

Some hooks are duplicated throughout the WP code-base (contain different parameters), so it is necessarily to tab through the options for some autocompletes.

Hooks names which start as a variable have been removed, for example `do_action($page_hook)`, there are not many in WP and there is no great way to add them to Sublime.

### Snippets

Snippets are slowly being added, to call a snippet you use the same function name, the autocomplete will show you and "ALL Options" selection. For example to
register a custom post type you would write `register_post...`

Current Snippets:

 - `plugin` : Creates plugin boilerplate
 - `register_post_type` : Register Post Type All Options 
 - `register_taxonomy`  : Register Taxonomy All Options
 - `wp_nav_menu` : wp_nav_menu All Options

### Tip

Sublime won't autocomplete PHP files when there is no closing `?>` tags , so in "Preferences-->Settings-User" add this snippet:

    "auto_complete_selector": "source, text",

### ToDo

Add more snippets


#### Manual
  
Download the .zip or git clone this into your sublime packages location, you can find it under "Preferences-->Browse Packages".

