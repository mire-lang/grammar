# Changelog

All notable changes to the Mire Grammar project will be documented in this file.

## [1.2.0] - 2026-11-14
### Changed
- **TextMate identity corrected.** The grammar name is `Mire` and the scope is
  `source.mire`; it previously shipped as `Grammar` / `source.grammar`, which
  made editors and Linguist treat it as an unrelated language.
- **`.mr` added to `fileTypes`.** Kioto and the compiler still use `.mr` for
  package sources, so both extensions now highlight.
- Grammar rules cover `load!`/`use!`, `mut`, `@[test]` attributes and `dasu`.

## [1.1.0] - 2026-09-17
### Added
- Initial release of Mire Grammar
- Complete syntax highlighting for Mire language (`*.mire`)
- Support for all language constructs defined in Avenys v1.1.0/SYNTAX.md
- Grammar compatible with GitHub Linguist and TextMate editors
- Comprehensive topic documentation in `docs/` directory
- Contribution guidelines and test procedures
- Backward compatibility guarantees

## [Older Versions]
- Pre-release versions and historical changes are tracked in git history

## Unreleased
- Planned improvements and bug fixes
