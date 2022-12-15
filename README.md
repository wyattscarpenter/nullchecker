# nullchecker

Blah blah blah, uh, actually do this project at some point.

I don't know if people already find this obvious, but a nullable pointer is a fine implementation of a Maybe/Optional type. Besides syntax, the only difference is how useful your type system is in giving you warnings about this stuff. So, nullchecker simply traces your pointer usages to make them just as typesafe as Maybes.

Nullchecker can be run in various modes, like enforcing that all pointers be nonnullable except for those explicitly marked as nullable (the default, which I recommend), or merely enforcing that all pointers marked as nonnullable can never be null (useful for gradually enforcing null-safety properties in an extant codebase).

There are three annotations supplied: @Nullable, @Nonnullable, & @Nonunnullable; the last of these indicates a pointer that can only ever be null.
