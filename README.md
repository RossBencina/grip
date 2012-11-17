Grip -- Github Readme Instant Preview
=====================================

Render local readme files before sending off to Github.

[http://github.com/joeyespo/grip](http://github.com/joeyespo/grip)


What is this?
-------------

Grip is a server written in Python that uses the Github
[markup API](http://developer.github.com/v3/markdown/)
to render a local readme. The styles also come directly
from Github, so you'll know exactly how it will appear.

The package includes both a command-line interface
and a Python API.


Why do you need it?
-------------------

Sometimes you just want to see the exact readme
result before committing and pushing to Github.


Usage
-----

The command-line interface is simple. Visit the directory of your readme, then:

    $ grip

Now open a browser and visit [`localhost:5000`](http://localhost:5000/)


API
---

You can access the API directly with Python, using it in your own projects:

    from grip import serve
    
    serve(directory='path-to-your-file')

Other functions include: `find_readme`, `render_content`, and `render_page`


Installation
------------

To install grip, simply:

    $ pip install grip
