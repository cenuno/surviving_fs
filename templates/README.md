# Templates

*Note: This comes directly from the [Templates section](http://flask.pocoo.org/docs/1.0/tutorial/templates/#templates) within the Flask documentation.*

The template files will be stored in the `templates` directory inside the flaskr package.

Templates are files that contain static data as well as placeholders for dynamic data. A template is rendered with specific data to produce a final document. Flask uses the [Jinja](http://jinja.pocoo.org/docs/templates/) template library to render templates.

In your application, you will use templates to render [HTML](https://developer.mozilla.org/docs/Web/HTML) which will display in the user’s browser. In Flask, Jinja is configured to autoescape any data that is rendered in HTML templates. This means that it’s safe to render user input; any characters they’ve entered that could mess with the HTML, such as `<` and `>` will be *escaped* with *safe* values that look the same in the browser but don’t cause unwanted effects.

Jinja looks and behaves mostly like Python. Special delimiters are used to distinguish Jinja syntax from the static data in the template. Anything between `{{` and `}}` is an expression that will be output to the final document. `{%` and `%}` denotes a control flow statement like `if` and `for`. Unlike Python, blocks are denoted by start and end tags rather than indentation since static text within a block could change indentation.

