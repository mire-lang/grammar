# Contributing to Mire Grammar

Thank you for considering contributing to the Mire grammar! This grammar provides syntax highlighting for the Mire programming language.

## How to Contribute

### Reporting Issues
- Check existing issues before creating a new one
- Include sample `.mire` code that demonstrates the issue
- Describe the expected vs. actual highlighting behavior

### Submitting Fixes
1. Fork the repository
2. Create a new branch (`git checkout -b fix/issue-description`)
3. Make your changes to `mire.tmLanguage.json`
4. Test with sample `.mire` files
5. Commit with clear description
6. Push and create a Pull Request

### Adding New Grammar Rules
1. Follow the existing pattern format in `mire.tmLanguage.json`
2. Use descriptive scope names
3. Test thoroughly with various `.mire` code snippets
4. Ensure no false positives or negatives
5. Update documentation if needed

### Code Review
- All contributions require review
- Ensure changes maintain backward compatibility
- Follow the existing code style and naming conventions
- Update documentation as needed

## Development Setup

1. Clone the repository
2. Install a TextMate-compatible editor (VS Code, Sublime Text, Atom)
3. Place `mire.tmLanguage.json` in the editor's grammar folder
4. Create test `.mire` files covering all syntax categories
5. Verify highlighting works correctly
5. Run the test suite if available

## Release Process

1. Update version in documentation if needed
2. Test all grammar rules with existing codebases
3. Changelog entries for user-visible changes
4. Tag the release version
5. Publish to grammar repository

## Versioning

This grammar follows [Semantic Versioning](https://semver.org/):
- **MAJOR**: Breaking changes to grammar rules
- **MINOR**: New syntax support without breaking changes
- **PATCH**: Bug fixes and pattern refinements

Current version: 1.1.0 (corresponds to Mire/Avenys v1.1.0+)
