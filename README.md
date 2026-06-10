# Blue Bolt 3D - Website Administration Guide

This repository hosts the public deployment for the Blue Bolt 3D rapid manufacturing intake portal. The site architecture uses a data-driven layout, completely decoupling the text copy from the HTML layout via an external JSON configuration file.

---

## 🛠️ How to Make Text Edits

To update pricing, lead times, machine specifications, or text captions across the website, you do not need to alter the HTML structures. 

1. Open the `content.json` file.
2. Edit the string values corresponding to the target layout sections.
   * *Note: Ensure standard JSON syntax formatting is preserved (keep matching double quotes and trailing commas).*
3. Use the **Live Server** extension in VS Code to locally preview and validate your formatting changes before pushing online.

---

## 🚀 Pushing Changes to the Live Website

Once you have verified your file edits or added new asset photographs to your project directory, open your VS Code terminal and execute the following deployment sequence:

```bash
# 1. Stage all new files and modified codebase changes
git add .

# 2. Lock in your save point with a descriptive update message
git commit -m "update: documentation refresh and text tweaks"

# 3. Stream the updates live to the GitHub Pages production server
git push