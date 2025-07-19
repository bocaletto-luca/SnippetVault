# SnippetVault

SnippetVault is a powerful, single-page code snippet manager that runs entirely in your browser. Store and organize your reusable code blocks with custom titles, tags, descriptions and full syntax highlighting. SnippetVault indexes every snippet for lightning-fast, full-text search using Lunr.js, supports multiple languages (JavaScript, HTML, CSS, Python, Markdown), and offers one-click copy, download and JSON export/import. No server or build step required—just open `index.html` in any modern browser to start saving your snippets offline, across devices, and securely in LocalStorage.

---

## Features

- Create, edit and delete unlimited code snippets  
- Syntax highlighting powered by CodeMirror (JS, HTML, CSS, Python, Markdown)  
- Full-text search with Lunr.js on title, tags, description and code  
- Tag management: comma-separated tags for categorization and filtering  
- One-click actions:  
  - 💾 Save/update snippet  
  - 🗑️ Delete snippet  
  - 📋 Copy code to clipboard  
  - ⬇️ Download snippet as file (`.js`, `.html`, `.css`, `.py` or `.md`)  
- Export all snippets as JSON for backup or sharing  
- Import a JSON backup to restore your entire snippet library  
- Light and Dark mode toggle for comfortable coding day or night  
- 100% client-side; zero dependencies on backend or build tools  
- Responsive layout works on desktop, tablet and mobile  

---

## Live Demo

Try SnippetVault in action via GitHub Pages:  
https://bocaletto-luca.github.io/SnippetVault/index.html

---

## Installation

No installation or build tools required. Simply clone the repository and open the file in your browser:

```bash
git clone https://github.com/bocaletto-luca/SnippetVault.git
cd SnippetVault
# Optionally serve with a static HTTP server:
python3 -m http.server 8000
# or
npx http-server . -p 8000
```

Then navigate to `http://localhost:8000/index.html` (or open `index.html` directly).

---

## Usage

1. **Create a new snippet**  
   - Click **+ New Snippet** in the sidebar.  
   - Fill in Title, select language, add Tags and a short Description.  
   - Write or paste your code in the editor panel.  
   - Click **💾 Save** to store the snippet.

2. **Browse and search snippets**  
   - Type keywords in the **Search** box for instant, full-text lookup across all snippets.  
   - Click any snippet title in the sidebar to load it for editing.

3. **Modify or delete**  
   - After loading a snippet, edit fields and click **💾 Save** to update.  
   - Click **🗑️ Delete** to permanently remove the current snippet.

4. **Copy or download**  
   - Use **📋 Copy Code** to copy the snippet text to your clipboard.  
   - Use **⬇️ Download** to save the snippet as a file with the appropriate extension.

5. **Backup & restore**  
   - Click **Export JSON** to download all snippets as a JSON file.  
   - Click **Import JSON** and select a previously exported file to restore.

6. **Dark/Light mode**  
   - Click **🌙 Dark Mode** to switch themes; click again to return to light.

---

## Customization

- **Themes & Colors**  
  Edit CSS variables in the `<style>` block of `index.html`:
  ```css
  :root {
    --primary: #0066cc;       /* Accent color */
    --bg: #f5f5f5;           /* Background color */
    --card: #ffffff;         /* Panel background */
    --text: #333333;         /* Base text color */
  }
  ```
- **Editor Settings**  
  Change CodeMirror options (theme, line numbers, indentation) in the script section.
- **Search Configuration**  
  Tweak Lunr.js indexing fields or boost weights in the `buildSearchIndex()` function.

---

## File Structure

```bash
SnippetVault/
├── index.html       # All-in-one single-page app (HTML, CSS, JS)
├── LICENSE          # GNU GPL v3.0 license
└── README.md        # Project documentation
```

---

## Contributing

Contributions, bug reports and feature requests are welcome!

1. Fork this repository  
2. Create a feature branch: `git checkout -b feature/my-feature`  
3. Commit your changes: `git commit -m "Add my awesome feature"`  
4. Push to your branch: `git push origin feature/my-feature`  
5. Open a Pull Request on GitHub

Please follow the existing code style and ensure compatibility across major browsers.

---

## License

This project is released under the **GNU General Public License v3.0** (GPL-3.0). See the [LICENSE](LICENSE) file for full terms.

---

## Author

**Bocaletto Luca**  
- GitHub: [@bocaletto-luca](https://github.com/bocaletto-luca)  
- Repository: [SnippetVault](https://github.com/bocaletto-luca/SnippetVault)
