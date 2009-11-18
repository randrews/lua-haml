# Lua Haml

## About

Lua Haml is an implementation of the [Haml](http://haml-lang.com) markup
language for Lua. Though it is implemented in Lua, its design makes it easily
adaptable to almost any language, and it includes an experimental renderer
for Haml for Ruby. Lua Haml is "just Haml," with no extending of the original
language.

A Haml language reference can be found
[here](http://haml-lang.com/docs/yardoc/HAML_REFERENCE.md.html).

Lua Haml currently supports the main features of Ruby's Haml, and can be used
for real work. However, many of the finer details of the language, some of them
important, are still being implemented.

### Working features

The following features of Ruby's Haml are working in Lua Haml:

* Options: format, autoclose, encoding
* Plain text
* Escapes
* HTML elements
* Ruby-style attributes
* HTML-style attributes
* Classes and id's (. and #)
* Implicit div elements
* Self-closing tags
* Doctypes and XML prologs
* Haml comments
* Code evaluation
* Ruby-style string interpolation ("#{var}")
* Running Lua
* Lua blocks
* Whitespace preservation (via filter)
* Filters: plain, javascript, preserve, escaped, lua, markdown, custom
* Partial templates. Lua Haml provides a simple default partial implementation,
	which can be overridden by frameworks as they see fit.
* HTML comments
* Conditional comments

### To do

The following features of Ruby's Haml are not yet working in Lua Haml:

* Options: escape\_html, suppress\_eval, attr\_wrapper, preserve
* Attribute methods
* Boolean attributes
* Whitespace removal
* Whitespace preservation (implicit)
* Escaping HTML
* Unescaping HTML
* Multiline content
* Helpers

The following features will likely not be implemented in Lua Haml:

* Object reference

To see an example of what you can do with the currently supported features, view
the "currently supported language" template in the spec directory.

I probably won't implement [Sass](http://sass-lang.com/) for a while yet,
possibly never. However if I do implement it, it will definitely be as a
separate project.

## Getting it

Install using LuaRocks:

    luarocks install luahaml --from=http://luarocks.org/repositories/rocks-cvs/

Don't be put off by the "CVS" in the URL, this will install the latest Lua Haml
from the stable branch on Github.


## Hacking it

The [Github repository](http://github.com/norman/lua-haml) is located at:

    git://github.com/norman/lua-haml.git

To run the specs, you should also install Telescope:

    luarocks install telescope --from=http://luarocks.org/repositories/rocks-cvs/

You can then run them using the ./bin/spec script in the repository.

## Bug reports

Please report them on the [Github issue tracker](http://github.com/norman/lua-haml/issues).

## Author

[Norman Clarke](mailto://norman@njclarke.com)

## Attributions

Some of the sample files in test/samples were taken from [Ruby's
Haml](http://github.com/nex3/haml/).

## Thanks

To Hampton Caitlin and Nathan Weizenbaum for their work on the original Haml.

## License

The MIT License

Copyright (c) 2009 Norman Clarke

Permission is hereby granted, free of charge, to any person obtaining a copy of
this software and associated documentation files (the "Software"), to deal in
the Software without restriction, including without limitation the rights to
use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
the Software, and to permit persons to whom the Software is furnished to do so,
subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS
OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
