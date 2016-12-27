# Reloaded C/C++

C/C++ must-have highlighter that understands many coding styles and APIs. Use with [Reloaded Themes](https://marketplace.visualstudio.com/items?itemName=reloadedextensions.reloaded-themes) extension that understands all the styles provided. This extension is C/C++ specific, but we are working on having all languages highlighted consistently.

The following concepts are provided:

  * It treats C/C++ the same way (no more separate colorizer for C).
  * It supports C and C++ keywords and always highlights them accordingly.
  * It provides configurability for many C/C++ keywords so they can be colorized differently.
  * It recognizes formatting of C/C++ strings like `"%d"` and `"\n"`.
  * It recognizes basic markdown and doxy-style commands in C/C++ comments.
  * It recognizes common types and constants of standard C library, Windows, Linux, and MAC.
  * It recognizes `assert()` and `YOUR_OWN_ASSERT()`-like macros.
  * It recognizes `likely()/unlikely()` and `YOUR_OWN_LIKELY()`-like macros.
  * It recognizes `IS_ERROR()` and similar macros for error handling.
  * It recognizes specific patterns in type/variable names, like `FirstUppercased`, `ALL_UPPERCASED`, and `typename_t`, these can be specified in themes and colorized differently.
  * It recognizes error constants like `kErr...`, `kError...` and `ERROR_...`.
  * Constants representing *success* and *failure* and can be highlighted differently.

NOTE: This extension doesn't provide code assistance, it just highlights concepts it understands. The extension should be considered experimental - PRs, suggestions, additions, and bug reports are welcome.

# License

This extension is based on official VSCode C/C++ extension, additions are licensed under MIT.
