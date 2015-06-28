Change Log
==========

Version 4.0.3 *(2015-06-27)*
----------------------------

 * Fix: Support trailing star-style comments (`/* hi */`) on enum values and fields.


Version 4.0.2 *(2015-06-27)*
----------------------------

 * Fix: Support uppercase "X" for hexademical notation prefix (e.g., "0XDEADBEEF").


Version 4.0.1 *(2015-06-09)*
----------------------------

 * Fix: Correctly handle equals sign between the 'syntax' keyword and its value.


Version 4.0.0 *(2015-05-25)*
----------------------------

 * New: Rewritten model to more accurately reflect the proto schema.
 * New: `DataType` interface and classes for representing type declarations.
 * New: Model classes all have a builder for creating instances.
 * New: `toSchema()` method renders model objects as proto schema.
 * New: Support for `oneof`, `map`, and `any` types.
 * New: Support for `syntax` declarations.
 * New: Option values are now always represented as a string, list, or map. The `kind()` of an
   option instance reflects the inferred type. This allows for correct representation of unsigned
   numbers and unknown enum values without special handling.


Version 3.1.5 *(2014-11-27)*
----------------------------

 * Fix: Honor the 'allow_alias' option when validating value tag uniqueness in enums.
 * Fix: Format multiple options on an enum value correctly in `toString()` output.
 * Fix: Add support for int, enum, and boolean option value types.
 * Fix: Preserve parenthesis specified around option names.


Version 3.1.4 *(2014-03-26)*
----------------------------

 * Fix: Enum duplicate scope check now correctly checks name instead of tag value.


Version 3.1.3 *(2014-03-25)*
----------------------------

 * Fix: Avoid NPE on deprecated, packed, and default field methods.


Version 3.1.2 *(2014-03-24)*
----------------------------

 * Fix: Extend declarations that are nested in other types are now properly supported.


Version 3.1.1 *(2014-02-13)*
----------------------------

 * Fix: Special-case Google's protobuf descriptors from the enum value constraint.


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
