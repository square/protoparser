Change Log
==========

Version 3.1.0 *(2014-01-02)*
----------------------------

 * New: `ScalarTypes` class with constants for each scalar type and `isScalarType` method.
 * New: Field values are now validated to be unique in their message.
 * New: Enum values are now validated to be unique in their parent scope.
 * New: `Option.findByName` convenience method for pulling options out of a list.
 * Fix: Correct parsing problem where the character immediately after a `;` was ignored.


Version 3.0.0 *(2013-12-30)*
----------------------------

 * New: Support for public imports.
 * New: `toString` emits valid proto syntax.
 * New: Services and enums now support type-level options.
 * New: Tag values are now checked to be valid.
 * New: All models now have public constructors.
 * New: `Type` now includes options list and documentation.
 * Options are now always presented as a list. Use `Option.optionsToMap` convenience method to
   convert them into a tree structure.
 * Fix: `equals` and `hashCode` for all models now properly checks all values.


Version 2.3.5 *(2013-11-04)*
----------------------------

 * New: Field options are available directly as a list.
 * New: Parse options defined on enum values.
 * Fix: Correctly parse option maps the lack commas.


Version 2.3.4 *(2013-10-23)*
----------------------------

 * Fix: Preserve leading whitespace on comments.


Version 2.3.3 *(2013-10-14)*
----------------------------

 * Fix: Disallow tag values less than or equal to zero.


Version 2.3.2 *(2013-09-12)*
----------------------------

 * Fix: Properly aggregate repeated option values.


Version 2.3.1 *(2013-09-10)*
----------------------------

 * Fix: Preserve square brackets in option names which denote extensions.


Version 2.3.0 *(2013-09-06)*
----------------------------

 * New: Support for values as lists.
 * New: Convenience methods for parsing from a `Reader` or `InputStream`.


Version 2.2.0 *(2013-09-03)*
----------------------------

 * New: Support for message options.


Version 2.1.1 *(2013-07-23)*
----------------------------

 * Fix: Properly parse escapes in quoted strings.


Version 2.1.0 *(2013-07-15)*
----------------------------

 * New: Support for fully-qualified names and extensions.
 * Fields on messages inside of extensions are now parsed properly.


Version 2.0.0 *(2013-06-06)*
----------------------------

 * Package is now `com.squareup.protoparser`.


Version 1.1.0 *(2013-04-27)*
----------------------------

 * New: Parse RPC service definitions.


Version 1.0.0 *(2013-02-01)*
----------------------------

Initial release.
