# material-theme-nikola
A theme for nikola based on Bootstrap 3 which lets you use the new [Google Material Design](http://www.google.com/design/spec/material-design/).

Based on [bootstrap-material-design](https://github.com/FezVrasta/bootstrap-material-design). Thank you!

![demo site](https://github.com/matuu/material-theme-nikola/blob/master/screenshots/screenshot-default.png)

See [demo](http://matuu.github.io/material-theme-nikola/).

## How use?

Simple. Copy dist/material-theme into the 'themes' folder into your project, and then you write 'material-theme' in theme option into your conf.py file.

That is all!

## Customization

This options must be specify in conf.py, into GLOBAL_CONTEXT variable:

### Navbar color schema 

    GLOBAL_CONTEXT = {                                                               
         'header_color': 'default'                                                    
    }

Options available:

* `default` or `primary`
* `success`
* `info`
* `warning`
* `danger`

![headers examples](https://github.com/matuu/material-theme-nikola/blob/master/screenshots/navbars.png)


### Social links in floating action button

    GLOBAL_CONTEXT = {
        "social_links": [
        {
            'bgcolor': "#F44336",
            'icon': "<i class='fa fa-share-square-o'></i>"
        },
        {
            "url": "https://twitter.com/",
            "bgcolor": "#55ACEE",
            "color": "#fffff",
            "icon": "<i class='fa fa-twitter'></i>",
            "target": "_blank"
        },
        {
            "url": "https://github.com/",
            "bgcolor": "#666666",
            "color": "#fffff",
            "icon": "<i class='fa fa-github-square'></i>",
            "target": "_blank"
        },
        {
            "url": "https://plus.google.com/",
            "bgcolor": "#DB4A39",
            "color": "#fffff",
            "icon": "<i class='fa fa-google-plus'></i>",
            "target": "_blank"
        },
        {
            "url": "https://www.facebook.com",
            "bgcolor": "#3B5998",
            "color": "#fffff",
            "icon": "<i class='fa fa-facebook'></i>",
            "target": "_blank"
        },
        ]
    }
    
![actions-links-collapsed](https://github.com/matuu/material-theme-nikola/blob/master/screenshots/actions-links1.png) ![actions-links-expanded](https://github.com/matuu/material-theme-nikola/blob/master/screenshots/actions-links2.png)


### Set author's avatar in header post

    GLOBAL_CONTEXT = {
        'author_avatar': '/images/avatar.jpg',
    }
    
![author's avatar](https://github.com/matuu/material-theme-nikola/blob/master/screenshots/avatar_author.png)


### Show author's biography into the dialog of credits (or footer)

For convenience, first define a variable with the html biography.

    BIOGRAPHY = """
    <img class="img-circle" style="float:left;margin:10px 20px 10px 0px;max-height:200px;" src="/images/avatar.jpg">
    <p>Nikola Tesla (Serbian Cyrillic: Никола Тесла; 10 July 1856 – 7 January 1943) was a Serbian American inventor, electrical engineer, mechanical engineer, physicist, and futurist best known for his contributions to the design of the modern alternating current (AC) electricity supply system.
    </p>
    """
    
Then, add it to `biography` viariable into `GLOBAL_CONTEXT`

    GLOBAL_CONTEXT = {
        "biography": BIOGRAPHY,
    }

![biography](https://github.com/matuu/material-theme-nikola/blob/master/screenshots/biography-demo.png)
