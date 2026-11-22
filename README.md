# Lyric Language Support

Official VS Code extension for the Lyric programming language. It provides syntax highlighting 
and editor configuration for `.ly` files.

## Features

### Syntax highlighting

- **Types and declarations**: `def`, `class`, `var`, `int`, `flt`, `str`, `god`, `bin`, `rex`, `arr`, `map`, `obj`, `dsk`, `pyobject`
- **Control flow**: `if`, `elif`, `else`, `case`, `given`, `for`, `done`, `end`, `try`, `catch`, `finally`, `fade`, `raise`, `import`, `importpy`, `break`, `continue`, `return`, `as`, `in`, `and`, `or`, `not`
- **Access modifiers**: `public`, `private`, `protected`
- **Inheritance**: `based on`
- **Built-in functions**: `print`, `input`, `range`, `open`, `type`, `isinstance`, `regex`, `exec`, `getopts`
- **Constants**: `true`, `false`, `True`, `False`, `None`
- **Numbers and strings**: numeric literals, single- and double-quoted strings, and escape sequences
- **Operators**: arithmetic, comparison, assignment, file I/O (`->`, `->>`, `<-`), and shell chain (`&&`, `||`, `|`)
- **Class terminator**: `+++`
- **Comments**: `#` line comments

### Editor configuration

- Bracket matching for `{}`, `()`, `[]`, and Lyric block pairs (`class` / `+++`, `try` / `fade`, `given` / `done`, `for` / `done`, `if` / `end`)
- Auto-closing quotes and brackets
- Folding for `class`, `try`, `given`, `for`, `if`, `case`, `else`, `catch`, and `finally` blocks
- Identifier word pattern for Lyric names

## Installation

From the repository root, with Node.js 20 or later:

```bash
npx @vscode/vsce package
```

vsce writes `lyric-lang-<version>.vsix` in the repository root. The filename comes from `name` and `version` in `package.json`. With the current manifest that file is `lyric-lang-0.8.5.vsix`.

1. Open the Extensions view (`Ctrl+Shift+X` on Windows and Linux, `Cmd+Shift+X` on macOS).
2. Open the **Views and More Actions...** menu (`⋮`) at the top of the Extensions view.
3. Choose **Install from VSIX...** and select the `.vsix` file.
4. Reload the window if VS Code asks you to.

From a terminal, with the `code` command on your `PATH`:

```bash
code --install-extension lyric-lang-<version>.vsix
```

To try the extension without packaging, open this folder in VS Code and press **F5**.

## Requirements

Visual Studio Code 1.80.0 or later.

## License

[MIT](LICENSE)

(c) 2026 MiraNova Studio
