# Static

This directory was created to store [`brython`](https://brython.info/static_doc/en/install.html) - Browser Python - JavaScript files.

## Installation

After running `mkdir static` in the Terminal, I downloaded `brython` via `pip install brython`. I then changed into the `static` directory before installing the necessary `brython` files via the following command:

```bash
python -m brython --install
```

## File Directory

| **File name** | **Description** |
| :-----------: | :-------------: |
| `brython.js` | the Brython engine, to include in the HTML page |
| `brython_stdlib.js` | groups all the modules and packages of the part of the Python standard library supported by Brython |
| `demo.html` | a page with a few examples of how to use Brython for client-side development |
| `unicode.txt` | a text file with [unicode](http://www.unicode.org/standard/WhatIsUnicode.html) translations |

### Demo Instructions

*Note: the following comes from the `README.txt` file that was created after running `python -m brython --install`. I've deleted it and placed its contents here.*

To run the demo, start the built-in Python HTTP server by

```bash
python -m brython --server
```

The default port is 8080. To specify another port:

```bash
python -m brython --server --port 8081
```

Then load http://localhost:<port>/demo.html in the browser address bar.

For more information please visit http://brython.info.
