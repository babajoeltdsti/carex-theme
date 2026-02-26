# 🎨 Carex Theme

<div align="center">

![Carex Theme Banner](https://img.shields.io/badge/Carex-Modern%20Theme-89b4fa?style=for-the-badge&logo=visual-studio-code&logoColor=white)

![Version](https://img.shields.io/visual-studio-marketplace/v/OMERBABACO.carex-theme?style=for-the-badge&color=89b4fa&label=Version)
![Downloads](https://img.shields.io/visual-studio-marketplace/d/OMERBABACO.carex-theme?style=for-the-badge&color=f38ba8&label=Downloads)
![Rating](https://img.shields.io/visual-studio-marketplace/r/OMERBABACO.carex-theme?style=for-the-badge&color=f9e2af&label=Rating)
![Installs](https://img.shields.io/visual-studio-marketplace/i/OMERBABACO.carex-theme?style=for-the-badge&color=cba6f7&label=Installs)

**A beautiful, modern VS Code theme inspired by Catppuccin. Available in Dark, Light, and High Contrast variants.**

[🚀 Install Now](https://marketplace.visualstudio.com/items?itemName=OMERBABACO.carex-theme) • [🐛 Report Bug](https://github.com/babajoeltdsti/carex-theme/issues) • [💡 Request Feature](https://github.com/babajoeltdsti/carex-theme/issues) • [⭐ Star on GitHub](https://github.com/babajoeltdsti/carex-theme)

</div>

---

## ✨ Features

<table>
<tr>
<td width="50%">

### 🎨 **Three Beautiful Variants**
Choose between Dark, Light, and High Contrast themes to match your environment and accessibility needs.

### 🌈 **Modern Color Palette**
Inspired by Catppuccin, featuring soft, eye-friendly colors that reduce strain during long coding sessions.

### 💎 **Comprehensive Styling**
400+ UI elements and 15+ syntax highlighting rules ensure every part of your editor looks perfect.

</td>
<td width="50%">

### 👁️ **Eye-Friendly Design**
Carefully selected colors and contrast ratios designed specifically to prevent eye fatigue.

### 🎯 **Multi-Language Support**
Optimized syntax highlighting for JavaScript, TypeScript, Python, React, Vue, and 20+ more languages.

### ♿ **Accessibility First**
High Contrast variant meets WCAG accessibility standards for users with visual impairments.

</td>
</tr>
</table>

---

## 🎨 Theme Variants

### 🌙 Carex Dark

Perfect for night coding and low-light environments.

**Color Palette:**
- Background: `#1e1e2e` - Soft dark purple-gray
- Foreground: `#cdd6f4` - Light lavender-white
- Accent: `#89b4fa` - Soft blue
- Keywords: `#f38ba8` - Soft pink
- Strings: `#a6e3a1` - Soft green
- Numbers: `#f9e2af` - Soft yellow
- Functions: `#89b4fa` - Soft blue
- Classes: `#cba6f7` - Soft purple

### ☀️ Carex Light

Ideal for daytime coding and bright environments.

**Color Palette:**
- Background: `#eff1f5` - Light gray-white
- Foreground: `#4c4f69` - Dark gray
- Accent: `#1e66f5` - Vibrant blue
- Keywords: `#d20428` - Vibrant red
- Strings: `#40a02b` - Vibrant green
- Numbers: `#df8e1d` - Vibrant orange
- Functions: `#1e66f5` - Vibrant blue
- Classes: `#8839ef` - Vibrant purple

### ⚡ Carex High Contrast

Maximum contrast for accessibility and outdoor use.

**Color Palette:**
- Background: `#000000` - Pure black
- Foreground: `#ffffff` - Pure white
- Accent: `#00ffff` - Pure cyan
- Keywords: `#ff0000` - Pure red
- Strings: `#00ff00` - Pure green
- Numbers: `#ffff00` - Pure yellow
- Functions: `#00ffff` - Pure cyan
- Classes: `#ff00ff` - Pure magenta

---

## 📦 Installation

### Method 1: VS Code Marketplace (Recommended)

1. Open **Extensions** sidebar in VS Code (`Ctrl+Shift+X` / `Cmd+Shift+X`)
2. Search for **"Carex"**
3. Click **Install**
4. Press `Ctrl+K Ctrl+T` / `Cmd+K Cmd+T` to open theme selector
5. Choose **Carex Dark**, **Carex Light**, or **Carex High Contrast**

### Method 2: Command Line

```bash
code --install-extension OMERBABACO.carex-theme
```

### Method 3: Quick Open

1. Press `Ctrl+P` / `Cmd+P`
2. Paste: `ext install OMERBABACO.carex-theme`
3. Press Enter

---

## 🖼️ Screenshots

### Carex Dark - JavaScript/TypeScript
```javascript
// Modern, soft colors for comfortable night coding
import { useState, useEffect } from 'react';

interface User {
  id: number;
  name: string;
  email: string;
}

async function fetchUserData(userId: string): Promise<User> {
  const response = await fetch(`/api/users/${userId}`);
  const data = await response.json();
  return data;
}

class UserManager {
  private users: User[] = [];
  
  constructor() {
    this.loadUsers();
  }
  
  async loadUsers(): Promise<void> {
    const users = await fetchUserData('all');
    this.users = users;
  }
}
```

### Carex Light - Python
```python
from typing import List, Dict, Optional
import asyncio

class DataProcessor:
    """Process data with modern, vibrant colors"""
    
    def __init__(self, name: str):
        self.name = name
        self._data: List[Dict] = []
        self._processed = False
    
    @property
    def is_processed(self) -> bool:
        """Check if data has been processed"""
        return self._processed
    
    async def process_async(self, items: List[str]) -> None:
        """Process items asynchronously"""
        for item in items:
            await asyncio.sleep(0.1)
            self._data.append({"item": item, "status": "processed"})
        self._processed = True
```

### Carex High Contrast - CSS
```css
/* Maximum contrast for accessibility */
.container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 24px;
  padding: 32px;
  background: linear-gradient(135deg, #00ffff, #ff00ff);
  border-radius: 16px;
  box-shadow: 0 8px 32px rgba(0, 255, 255, 0.3);
}

.button {
  background: #00ff00;
  color: #000000;
  border: 2px solid #ffff00;
  padding: 12px 24px;
  font-weight: bold;
  transition: all 0.3s ease;
}

.button:hover {
  background: #ffff00;
  transform: translateY(-2px);
  box-shadow: 0 12px 40px rgba(255, 255, 0, 0.5);
}
```

---

## ⚙️ Recommended Settings

For the best experience with Carex themes, add these settings to your `settings.json`:

```json
{
  // Font settings
  "editor.fontFamily": "'Fira Code', 'JetBrains Mono', 'Cascadia Code', 'SF Mono', Consolas, monospace",
  "editor.fontLigatures": true,
  "editor.fontSize": 14,
  "editor.lineHeight": 22,
  "editor.letterSpacing": 0.5,
  
  // Cursor settings
  "editor.cursorBlinking": "smooth",
  "editor.cursorSmoothCaretAnimation": "on",
  "editor.cursorStyle": "line",
  "editor.cursorWidth": 2,
  
  // Bracket settings
  "editor.bracketPairColorization.enabled": true,
  "editor.guides.bracketPairs": true,
  "editor.guides.bracketPairsHorizontal": "active",
  
  // Editor appearance
  "editor.renderWhitespace": "boundary",
  "editor.renderLineHighlight": "all",
  "editor.smoothScrolling": true,
  "editor.minimap.enabled": true,
  "editor.minimap.renderCharacters": false,
  
  // Workbench settings
  "workbench.iconTheme": "material-icon-theme",
  "workbench.productIconTheme": "material-product-icons",
  
  // Terminal settings
  "terminal.integrated.fontFamily": "'Fira Code', 'JetBrains Mono', monospace",
  "terminal.integrated.fontSize": 13,
  "terminal.integrated.lineHeight": 1.3
}
```

---

## 🎯 Supported Languages

<table>
<tr>
<td width="33%">

### Web Development
- ✅ JavaScript
- ✅ TypeScript
- ✅ JSX / TSX
- ✅ HTML / XML
- ✅ CSS / SCSS / LESS
- ✅ JSON / JSONC
- ✅ YAML

</td>
<td width="33%">

### Backend & Systems
- ✅ Python
- ✅ Node.js
- ✅ PHP
- ✅ Ruby
- ✅ Go
- ✅ Rust
- ✅ C / C++ / C#
- ✅ Java

</td>
<td width="33%">

### Frameworks & Tools
- ✅ React
- ✅ Vue
- ✅ Angular
- ✅ Svelte
- ✅ SQL
- ✅ GraphQL
- ✅ Markdown
- ✅ Shell Script

</td>
</tr>
</table>

---

## 🔧 Customization

You can easily customize Carex theme colors in your `settings.json`:

### Change Background Color
```json
{
  "workbench.colorCustomizations": {
    "[Carex Dark]": {
      "editor.background": "#1e1e2e",
      "sideBar.background": "#181825"
    },
    "[Carex Light]": {
      "editor.background": "#eff1f5",
      "sideBar.background": "#e6e9ef"
    }
  }
}
```

### Customize Syntax Colors
```json
{
  "editor.tokenColorCustomizations": {
    "[Carex Dark]": {
      "comments": "#6c7086",
      "strings": "#a6e3a1",
      "keywords": "#f38ba8",
      "functions": "#89b4fa"
    },
    "[Carex Light]": {
      "comments": "#9ca0b0",
      "strings": "#40a02b",
      "keywords": "#d20428",
      "functions": "#1e66f5"
    }
  }
}
```

---

## 🆚 Comparison

<table>
<tr>
<th>Feature</th>
<th>Carex Dark</th>
<th>Carex Light</th>
<th>Carex High Contrast</th>
</tr>
<tr>
<td>Best For</td>
<td>Night coding</td>
<td>Day coding</td>
<td>Accessibility</td>
</tr>
<tr>
<td>Eye Strain</td>
<td>✅ Minimal</td>
<td>✅ Minimal</td>
<td>✅ Minimal</td>
</tr>
<tr>
<td>Contrast</td>
<td>Medium</td>
<td>Medium</td>
<td>Maximum</td>
</tr>
<tr>
<td>Color Style</td>
<td>Soft pastels</td>
<td>Vibrant</td>
<td>Pure colors</td>
</tr>
<tr>
<td>WCAG Compliant</td>
<td>AA</td>
<td>AA</td>
<td>AAA</td>
</tr>
</table>

---

## ❓ FAQ

<details>
<summary><strong>Q: Which variant should I use?</strong></summary>
<br>
A: Use <strong>Carex Dark</strong> for night coding or low-light environments, <strong>Carex Light</strong> for daytime or bright environments, and <strong>Carex High Contrast</strong> if you need maximum contrast for accessibility or outdoor use.
</details>

<details>
<summary><strong>Q: Can I use this theme with other icon themes?</strong></summary>
<br>
A: Absolutely! Carex works great with any icon theme. We recommend Material Icon Theme or Atom Material Icons for the best visual experience.
</details>

<details>
<summary><strong>Q: Does this theme support semantic highlighting?</strong></summary>
<br>
A: Yes! All Carex variants fully support VS Code's semantic highlighting feature, providing even more detailed and accurate syntax coloring.
</details>

<details>
<summary><strong>Q: Is this theme inspired by Catppuccin?</strong></summary>
<br>
A: Yes! Carex is heavily inspired by the beautiful Catppuccin color palette, specifically Mocha (Dark) and Latte (Light) variants, with our own unique touches.
</details>

<details>
<summary><strong>Q: How do I switch between variants?</strong></summary>
<br>
A: Press <code>Ctrl+K Ctrl+T</code> (or <code>Cmd+K Cmd+T</code> on Mac) to open the theme selector, then choose your preferred Carex variant.
</details>

<details>
<summary><strong>Q: Can I customize the colors?</strong></summary>
<br>
A: Yes! Check the <a href="#-customization">Customization section</a> above for examples of how to override colors in your settings.json.
</details>

---

## 🤝 Contributing

We love contributions! Here's how you can help:

1. 🐛 **Report Bugs** - Found an issue? [Open a bug report](https://github.com/babajoeltdsti/carex-theme/issues/new?template=bug_report.md)
2. 💡 **Suggest Features** - Have an idea? [Request a feature](https://github.com/babajoeltdsti/carex-theme/issues/new?template=feature_request.md)
3. 🔧 **Submit PRs** - Want to contribute code? Fork and submit a pull request!
4. ⭐ **Star the Repo** - Show your support on [GitHub](https://github.com/babajoeltdsti/carex-theme)
5. 📢 **Spread the Word** - Share Carex with your friends and colleagues!

---

## 📝 Changelog

See [CHANGELOG.md](CHANGELOG.md) for a detailed list of changes and version history.

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 💖 Acknowledgments

- Inspired by [Catppuccin](https://github.com/catppuccin/catppuccin) - An amazing color palette
- Thanks to the VS Code team for creating an incredible editor
- Special thanks to all contributors and users for their feedback and support
- Color theory and accessibility guidance from WCAG standards

---

## 🌟 Show Your Support

If you enjoy using Carex theme, please consider:

- ⭐ [Starring the repository](https://github.com/babajoeltdsti/carex-theme)
- 📝 [Writing a review](https://marketplace.visualstudio.com/items?itemName=OMERBABACO.carex-theme&ssr=false#review-details)
- 🐦 Sharing on social media
- ☕ [Buying us a coffee](https://buymeacoffee.com/babajoeltdsti) (optional)

---

<div align="center">

**[🚀 Install Now](https://marketplace.visualstudio.com/items?itemName=OMERBABACO.carex-theme)** • **[⭐ Star on GitHub](https://github.com/babajoeltdsti/carex-theme)** • **[🐛 Report Bug](https://github.com/babajoeltdsti/carex-theme/issues)** • **[💬 Discussions](https://github.com/babajoeltdsti/carex-theme/discussions)**

Made with 💜 by developers, for developers

**Happy Coding with Carex! 🎨✨**

</div>
