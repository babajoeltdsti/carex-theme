# Contributing to Carex Theme

First off, thank you for considering contributing to Carex Theme! 🎉

## 🤝 How Can I Contribute?

### 🐛 Reporting Bugs

Before creating bug reports, please check the existing issues to avoid duplicates. When you create a bug report, include as many details as possible:

- Use a clear and descriptive title
- Describe the exact steps to reproduce the problem
- Provide specific examples
- Describe the behavior you observed and what you expected
- Include screenshots if applicable
- Include your environment details (OS, VS Code version, theme variant)

### 💡 Suggesting Features

Feature requests are welcome! Please provide:

- A clear and descriptive title
- A detailed description of the proposed feature
- Explain why this feature would be useful
- Include mockups or examples if possible

### 🔧 Pull Requests

1. Fork the repository
2. Create a new branch (`git checkout -b feature/amazing-feature`)
3. Make your changes
4. Test your changes thoroughly
5. Commit your changes (`git commit -m 'Add some amazing feature'`)
6. Push to the branch (`git push origin feature/amazing-feature`)
7. Open a Pull Request

#### Pull Request Guidelines

- Follow the existing code style
- Update documentation if needed
- Test all three theme variants (Dark, Light, High Contrast)
- Ensure colors maintain accessibility standards
- Keep commits atomic and well-described

## 🎨 Theme Development

### Project Structure

```
carex-theme/
├── themes/
│   ├── carex-dark.json          # Dark variant
│   ├── carex-light.json         # Light variant
│   └── carex-high-contrast.json # High Contrast variant
├── icon.png                      # Extension icon
├── package.json                  # Extension manifest
├── README.md                     # Documentation
├── CHANGELOG.md                  # Version history
└── LICENSE                       # MIT License
```

### Color Guidelines

**Carex Dark (Catppuccin Mocha inspired)**
- Use soft, pastel colors
- Maintain medium contrast
- Background should be dark but not pure black
- Colors should be easy on the eyes

**Carex Light (Catppuccin Latte inspired)**
- Use vibrant but not harsh colors
- Maintain good contrast with light background
- Background should be light but not pure white
- Colors should be clear and readable

**Carex High Contrast**
- Use pure, saturated colors
- Maximum contrast for accessibility
- Must meet WCAG AAA standards
- Pure black background, pure white text

### Testing Your Changes

1. Press `F5` in VS Code to open Extension Development Host
2. Test all three variants
3. Check multiple file types (JS, TS, Python, HTML, CSS, etc.)
4. Verify UI elements (sidebar, tabs, status bar, etc.)
5. Test in different lighting conditions

### Building the Extension

```bash
# Install dependencies
npm install

# Package the extension
npm run package

# This creates a .vsix file you can install locally
```

## 📝 Code of Conduct

### Our Pledge

We are committed to providing a welcoming and inspiring community for all.

### Our Standards

- Be respectful and inclusive
- Accept constructive criticism gracefully
- Focus on what's best for the community
- Show empathy towards others

### Unacceptable Behavior

- Harassment or discriminatory language
- Trolling or insulting comments
- Personal or political attacks
- Publishing others' private information

## 📜 License

By contributing, you agree that your contributions will be licensed under the MIT License.

## 🙏 Thank You!

Your contributions make Carex Theme better for everyone. We appreciate your time and effort!

---

**Questions?** Feel free to reach out by opening an issue or discussion on GitHub.
