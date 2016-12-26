# Reloaded C/C++

C/C++ must-have colorizer that understands many coding styles and APIs. This extension should be used with "Reloaded Themes" theme as the theme understands and colorizes many tokens that this extension provides. It's C/C++ specific, but we are working on having all languages colorized consistently.

The following concepts are provided:

  * It treats C/C++ the same way (no more separate colorizer for C).
  * It supports C and C++ keywords and always highlights them accordingly.
  * It provides configurability for many C/C++ keywords so they can be colorized differently.
  * It recognizes common types and constants of standard C library, Windows, Linux, and MAC.
  * It recognizes "assert()" and "YOUR_OWN_ASSERT()"-like macros.
  * It recognizes "likely()/unlikely()" and "YOUR_OWN_LIKELY()"-like macros.
  * It recognizes "IS_ERROR()" and similar macros for error handling.
  * It recognizes specific patterns in type/variable names, like 'FirstUppercased', 'ALL_UPPERCASED', and 'typename_t', these can be specified in themes and colorized differently.
  * It recognizes error constants like "kError..." and "ERROR_...".
  * Error constants are categorized to "success" and "failure" and can be colored differently.

The extension should be considered experimental - PRs, suggestions, bug reports are welcome.

# License

This extension is based on official VSCode C/C++ extension, additions are licensed under MIT.
