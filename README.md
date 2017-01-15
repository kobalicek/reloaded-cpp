# Reloaded C/C++

Extension that replaces the built-in C/C++ tokenizer (grammar) with a custom one that provides more styles than the default one. Use with [Reloaded Themes](https://marketplace.visualstudio.com/items?itemName=reloadedextensions.reloaded-themes) extension that understands everything this tokenizer provides.

The following concepts are provided:

  * It treats C/C++ the same way (no more separate grammar for C, the reason was that H files were always tokenized as C++ anyway, so there was no point of maintaining two grammars).
  * It supports C and C++ keywords and provides styles so these can be highlighted individually (you can highlight inline differently than extern, for example).
  * It recognizes formatting and escaping of C/C++ strings like `"%d"` and `"\n"`, respectively.
  * It recognizes basic markdown and doxy-style commands in C/C++ comments, both `\\` and `@` doxygen escapes are recognized.
  * It recognizes common types and constants of standard C library, Windows, Linux, and MAC.
  * It recognizes `assert()` and `YOUR_OWN_ASSERT()`-like macros.
  * It recognizes `likely()/unlikely()` and `YOUR_OWN_LIKELY()`-like macros.
  * It recognizes `IS_ERROR()`, `SUCCEEDED()`, and similar macros for error handling.
  * It recognizes specific patterns in type/variable names, like `FirstUppercased`, `ALL_UPPERCASED`, and `typename_t`, these can be specified in themes and styled differently.
  * It recognizes error constants like libc's `ESOMETHING`, `kErr...`, `kError...`, and `ERROR_...`.
  * It recognizes success constants like `noErr`, `ERROR_OK`, `kNoErr`, `kErrorOk`, etc...
  * Constants representing *success* and *failure* and can be highlighted differently.
  * Many other improvements you may find useful.

# Important

  * Reloaded C/C++ 0.1.1+ requires at least vscode-1.9 as the styling in vscode was changed (this extension was updated to support these changes).
  * This extension doesn't provide code assistance, it just provides styles for concepts it understands, however, this extension can be used together with extensions providing code-assistance (just check out extensions that utilize clang for code assistance).
  * This extension should be considered experimental - contributions are welcome.

# License

This extension is based on official VSCode C/C++ tokenizer/grammar (which is based on textmate-cpp tokenizer/grammar), additions are licensed under MIT.
