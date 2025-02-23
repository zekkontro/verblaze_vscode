# Verblaze Translation Manager for VS Code

A powerful translation management extension for VS Code that helps you manage your translations directly within your development environment.

## Features

- 🔐 Easy login with CLI Token
- 🌍 Quick translation of selected text
- 🔍 Search through existing translations
- ⚡ Fast translation from context menu
- 📁 Automatic file translation

## Installation

1. Search for "Verblaze Translation Manager" in VS Code's Extension Marketplace
2. Click the "Install" button
3. Restart VS Code

## Usage

1. Open Command Palette (Mac: `Cmd+Shift+P`, Windows: `Ctrl+Shift+P`)
2. Run "Verblaze: Login with CLI Token" command
3. Enter your CLI Token
4. You can now start translating:
   - Right-click on selected text and choose "Translate Selection"
   - Use "Search Translations" from Command Palette
   - Use "Translate File" to automatically translate all strings in a file

### Translate File Feature

The Translate File feature automatically detects and translates all translatable strings in your current file. Here's how to use it:

1. Open the file you want to translate
2. Open Command Palette and run "Verblaze: Translate File" command
3. The extension will:
   - Automatically detect the file type
   - Find all translatable strings
   - Skip already translated strings (in format `file_key.value_key`)
   - Skip locked translations
   - Replace detected strings with their translation keys

Supported file types:

- React/Next.js (`.jsx`, `.tsx`, `.js`, `.ts`)
- React Native (`.jsx`, `.tsx`, `.js`, `.ts`)
- Flutter (`.dart`)
- Swift (`.swift`)
- Kotlin (`.kt`, `.kts`)
- Blazor (`.razor`, `.cshtml`)
- Qt (`.qml`)

The extension will detect:

- String literals (both single and double quotes)
- Template literals
- JSX text nodes
- UI-specific patterns (e.g., SwiftUI text attributes, Android XML attributes)

## Requirements

- VS Code 1.85.0 or higher
- Verblaze CLI Token

## License

ISC License

## Support

For any issues or suggestions, please visit our [GitHub Issues](https://github.com/verblaze/verblaze-vscode/issues) page.
