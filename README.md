# TinZ_Types_Manager


A browser-based XML editor designed for editing DayZ `types.xml` and mod files. This tool allows users to load multiple XML files, edit item attributes with undo/redo support, merge mod files into a base file with conflict resolution options, and export the updated XML.

## Features

- Load multiple XML files simultaneously for comparison and editing.
- Editable fields include nominal, lifetime, restock, min, category, usage, tag, and tier.
- Bulk edit options with percentage adjustments or direct value sets.
- Select/deselect individual or all items per page.
- Undo and redo changes with keyboard shortcuts (Ctrl+Z / Ctrl+Y).
- Merge mod files into a base file with customizable conflict handling.
- Export the base XML file with all applied changes.
- Pagination and filtering support for large datasets.
- Accessible and keyboard-navigable UI components.

## Usage

1. Open `index.html` in a modern browser (Chrome, Firefox, Edge).
2. Use the **Choose Files** button to load one or more DayZ XML files.
3. Select which file is the **Base** file; others will be treated as mods.
4. Edit individual entries inline or apply bulk edits to selected items.
5. Use the merge function to combine mods into the base file with conflict options.
6. Export the merged base file for use in your DayZ mods.

## Keyboard Shortcuts

- **Ctrl+Z / Cmd+Z** — Undo last change
- **Ctrl+Y / Cmd+Shift+Z** — Redo last undone change

## Development

- The entire editor runs client-side with no server dependencies.
- The main logic is contained within the `index.html` file.
- Future improvements planned: file selection UI, drag-and-drop uploads, better merge conflict UI.

## Contributing

Contributions, issues, and feature requests are welcome. Please open issues or pull requests on the repository.

## License

[MIT License](LICENSE) — Feel free to use and modify this project as you see fit.

---

### Step 3: GitHub Setup Instructions

If you have Git installed locally, you can create the repo and push your file as follows:

```bash
mkdir dayz-xml-editor
cd dayz-xml-editor
git init
echo "node_modules/" > .gitignore  # optional, if you add dependencies later
# Save your HTML file as index.html in this folder

# Create README.md with the content above
cat > README.md << EOF
[Paste the README content here]
EOF

git add index.html README.md .gitignore
git commit -m "Initial commit: DayZ XML Editor with basic functionality"
# Create a remote repo on GitHub (use the GitHub UI or CLI)
git remote add origin https://github.com/yourusername/dayz-xml-editor.git
git push -u origin master
