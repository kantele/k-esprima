**esprima-derby** ([esprima.org](http://esprima.org), BSD license)

This fork of Esprima is modified to parse expressions in Derby templates. Parsing of statements and other non-expression language features has been removed. ECMAScript keywords have been removed, so expressions such as `class` will be parsed as identifiers instead of as keywords.

In addition, a few modifications have been made to identifiers:

  * Identifiers may start with an at sign (`@`) or hash (`#`) in addition to the standard set of starting characters (underscore, dollar sign, A-Z, a-z, and ISO 8859-1 or Unicode characters)
  * After the first character, dentifiers may contain hyphens (`-`) in addition to the standard set of subsequent characters (underscore, dollar sign, A-Z, a-z, ISO 8859-1 or Unicode characters, and 0-9). Because of this extension, the expression `x-y` is interpreted as a single identifier, whereas `x - y` and `x -y` are interpreted as "`x` minus `y`".

For more information, see [derbyjs.com](http://derbyjs.com) and [esprima.org](http://esprima.org).
