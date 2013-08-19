## WordPress Sublime Text 2

This adds autocomplete for WordPress functions, hooks and constants.

### Notes

The other WordPress sublime package was not up to date and missing stuff so I build a custom parser for grabbing data from WP core, so it can stay in tune with the WP release cycle.

    Current WP version : 3.6  
    Auto completes     : 3284

There are no snippets added to this package, you would not remember them anyhow. Depreciated functions have been removed :smiley_cat:  

'To-do: Add WP Class's' 

### Tip

Sublime has issues with autcompleting php files that do not have closing `?>` tags , so in "Preferences-->Settings-User" add this snippet:

    "auto_complete_selector": "source, text",

### Installation

#### With Package Control

You can install Wordpress Autocomplete from inside Sublime Text itself. Open the Command Palette and select "Package Control: Install Package", then search for "Wordpress Autocomplete" and you're done!

#### Manual
  
Download the .zip or git clone this into your sublime packages location, you can find it under "Preferences-->Browse Packages".
   
You should have this instead: [package_control](http://wbond.net/sublime_packages/package_control)
