## WordPress Sublime Text 2

This adds autocomplete for WordPress Functions, Hooks, Constants and Classes for Sublime Text 2

### Notes

The other WordPress sublime package was not up to date and missing stuff so I build a custom parser for grabbing data from WP core.

    Current WP version : 3.6
     
    Functions  : 3165
    Hooks      : 1544
    Contants   :  121
    Classes    :   74


Depreciated functions have been removed :smiley_cat:  

Many hooks are duplictated (and also have same name as coorespoding function) because they contain differant parameters, so it is necesarry to tab through the options.

Hooks names which start as a variable have been removed, for example `do_action($page_hook)`, there is not many of these in WP.

*There might be some slight issues with hook completions due them being inconsistnly named by WP.*


### Tip

Sublime won't autcompleting PHP files that do not have closing `?>` tags , so in "Preferences-->Settings-User" add this snippet:

    "auto_complete_selector": "source, text",

### Installation

#### Manual
  
Download the .zip or git clone this into your sublime packages location, you can find it under "Preferences-->Browse Packages".
   
