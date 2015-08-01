# material-theme-nikola
A theme for nikola based on Bootstrap 3 which lets you use the new [Google Material Design](http://www.google.com/design/spec/material-design/).

Based on [bootstrap-material-design](https://github.com/FezVrasta/bootstrap-material-design).

## How use?

Simple. Copy dist/material-theme into the 'themes' folder into your project, and then you write 'material-theme' in theme option into your conf.py file.

That is all!

## Customization

#### Navbar's color schema 

In conf.py file:

    GLOBAL_CONTEXT = {                                                               
         'header_color': 'default'                                                    
    }

Options available:

* default or primary
* success
* info
* warning
* danger


