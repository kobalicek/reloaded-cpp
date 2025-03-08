# Reloaded C/C++

Extension that replaces the built-in C/C++ tokenizer/grammar and introduces additional tokens that can be styled. This extension should be used together with [Reloaded Themes](https://marketplace.visualstudio.com/items?itemName=reloadedextensions.reloaded-themes) extension as the additional tokens are new and not recognized by other themes!

# Deprecated

  * THIS EXTENSION IS DEPRECATED. It was written at a time when there was very little customization in vscode. Now it't much better and this extension doesn't provide anything that cannot be set in user config now. Please don't use this extension anymore.

# Important

  * This extension DOES NOT provide code assistance, it just recognizes common patterns used in today's C++ code.
  * This extension is experimental and should be used only with themes that understand the additional tokens it recognizes. If you don't use a compatible theme there is no point of using this extension.
  * Suggestions are welcome, if you think about more tokens / symbols to be recognized please fill an issue.

# Concepts provided

  * It treats C/C++ the same way (no more separate grammar for C, the reason was that header files were already tokenized as C++ anyway, so there was no point of maintaining two grammars).
  * It supports C and C++ keywords and provides styles so each keyword can be highlighted individually (you can highlight inline differently than extern, for example).
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

# License

This extension is based on official VSCode C/C++ tokenizer/grammar (which is based on textmate-cpp tokenizer/grammar), additions are licensed under MIT.
