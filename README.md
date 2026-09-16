# Mire Grammar

Syntax highlighting grammar for the Mire programming language (`.mire`), used by GitHub Linguist and compatible editors.

This grammar is independent from the compiler implementation and is distributed under the MIT license.

## Linguist Integration

GitHub Linguist uses this grammar to auto-detect `.mire` files in repositories. The grammar is properly configured for Linguist with:

- **File extension**: `.mire`
- **Scope name**: `source.grammar`
- **Language name**: `Mire`

Linguist will automatically:
- Detect `.mire` files in repositories
- Apply syntax highlighting in GitHub code views
- Distinguish `.mire` from other extensions
- Report language statistics in repository analytics

## Grammar Structure

The grammar is implemented as a TextMate grammar (`mire.tmLanguage.json`). It provides:

- Syntax highlighting for all Mire language constructs
- Scope names for accurate editor integration
- Pattern matching for language features
- Support for the `.mire` file extension

The grammar is located at `grammar/mire.tmLanguage.json` and follows the standard TextMate grammar format.

## Supported Language Features

This grammar highlights the following Mire language constructs:

- **Comments**: `//` line comments, `/! ... !/` block comments
- **Attributes**: `@[test]`, `@[macro!]`, `@[deprecated]`, `@[allow]`, `@[deny]`
- **Variables**: `set name = value`, `set name :type mut`, constants `:type const`
- **Types**: `i8/16/32/64/128`, `u8/16/32/64/128`, `f32/f64`, `bool`, `str`, `char`, `ptr`, `anything`, `arr`, `map`, `vec`, `maybe`, `result`
- **Type modifiers**: `const`, `mut`, `extern`, `fn`
- **Constants**: `true`, `false`, `none`, `some`, `ok`, `err`
- **Function declarations**: `fn name: (params) :return_type { body }`
- **Pipeline operators**: `=>` (discard), `?=>` (keep result)
- **Struct declarations**: `struct Name { field1 :type, field2 :type }`
- **Struct methods**: `impl Name { fn method(self) :type { ... } }`
- **Inheritance**: `struct Child extends Parent`
- **Enum declarations**: `enum Name { Variant1(payload), Variant2 }`
- **Enum matching**: `match expr { Variant(payload) => ... }`
- **Skill declarations**: `skill Name { fn method(self) :type }`
- **Skill inheritance**: `super ParentSkill`
- **Generics**: `fn name<T: Trait>(param :T) :ReturnType`
- **Control flow**: `if/else`, `while`, `for`, `find`, `do/while`
- **Pattern matching**: `match expr { pattern => ... }`
- **String interpolation**: `"Hello {name}!"`
- **Operators**: `+`, `-`, `*`, `/`, `%`, `==`, `!=`, `<`, `>`, `&&`, `||`, `!`, `|`, `&`, `^`, `~`, `<<`, `>>`
- **Pipeline**: `=>` (discard), `?=>` (keep result)
- **Module system**: `load module`, `load! module`, `module::function`
- **FFI declarations**: `extern fn name :type lib "library"`
- **Test framework**: `@[test]`, `@[section("name")]`, `@[ignore]`, `@[deprecated]`
- **Built-in functions**: `dasu`, `ireru`, `print`, `len`, `abs`, `sqrt`, etc.

## Documentation

- **CONTRIBUTING.md**: Contribution guidelines
- **CHANGELOG.md**: Version history
- **docs/**: 20 topic areas covering all Mire syntax constructs

## Versioning

This grammar follows Semantic Versioning:
- **MAJOR**: Breaking changes to grammar rules
- **MINOR**: New syntax support without breaking changes
- **PATCH**: Bug fixes and pattern refinements

Current version: 1.1.0 (corresponds to Mire/Avenys v1.1.0+)

## License

MIT License - See LICENSE file for details.

## Contact

For questions or contributions, please refer to the Avenys project channels or open an issue in this repository.
