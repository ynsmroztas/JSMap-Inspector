# JSMap Inspector ✨

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

**A powerful, offline, single-file HTML tool designed for developers and security researchers to inspect and analyze JavaScript Source Map (`.js.map`) files.**

Modern web applications often bundle and minify their JavaScript code. While this is great for performance, the associated source map files can inadvertently expose the original source code, including comments, variable names, and potentially sensitive information. JSMap Inspector provides a user-friendly interface to navigate this exposed code, search for critical data, and understand the structure of the bundled application – **all completely offline within your browser.**

![JSMap Inspector Screenshot](JSMapInspector.png.jpg) 
*(Replace with a compelling screenshot of the tool in action)*

---

## Features 🚀

* **📂 Load `.map` Files:** Easily load `.js.map` files using the file browser or simply **drag and drop** them onto the window.
* **🌳 Interactive Tree View:** Navigate the original source code structure with a familiar file/folder tree.
    * **✨ SVG File Icons:** Language-specific icons (JS, TS, JSON, CSS, HTML, etc.) for quick identification.
    * **↔️ Expand/Collapse Controls:** Quickly expand or collapse all folders in the tree.
    * **🖱️ Context Menu:** Right-click on files/folders to **Copy Path** or **Download File**.
* **📑 Tabbed Code Preview:** Open multiple files in tabs for easy comparison.
    * **🎨 Syntax Highlighting:** Code is automatically highlighted using Highlight.js (Monokai Sublime theme).
    * **📜 Word Wrap:** Toggle word wrapping for long lines, especially useful for minified code snippets.
* **🔍 Powerful Regex Search:** Search across all files within the source map using regular expressions.
    * **⚡ Predefined Critical Patterns:** Includes a comprehensive list of regex patterns specifically targeting sensitive information like:
        * API Keys & Secrets (Generic, AWS, Google Cloud)
        * Tokens (Generic, JWT)
        * Passwords
        * Private Key Blocks (RSA, EC, PGP, OpenSSH)
        * Database Connection Strings
        * Internal IP Addresses
        * Email Addresses
        * Developer Comments (TODO, FIXME, HACK)
    * **💻 Terminal-Style Output:** Search results are presented in a grouped, `grep`-like format showing the file path, line number, and highlighted code snippet.
    * **➡️ Jump to Line:** Clicking a search result snippet opens the file and scrolls directly to the matching line.
* **🌐 Domain Extraction:** Quickly extract all unique domain names found within the source code.
* **↔️↕️ Resizable Panes:** Adjust the size of the Tree View, Code Preview, and Results Panel using draggable splitters.
* **🎨 Themed UI:** Sleek, hacker-inspired dark theme with subtle neon glow effects and scanlines for a professional feel.
* **🔒 Offline & Single File:** Runs entirely in your browser. No server-side components, no data leaves your machine. Just download the single `JSMap-Inspector.html` file.

---

## Getting Started 🏁

1.  **Download:** Save the `JSMap-Inspector.html` file to your local machine.
2.  **Open:** Double-click the HTML file to open it in your preferred web browser (Chrome, Firefox, Edge recommended).
3.  **Load:**
    * Click the "**Browse...**" button (`input type="file"`) and select a `.js.map` file.
    * OR, **drag and drop** a `.js.map` file anywhere onto the browser window.

---

## Usage Guide 🧭

* **Browsing Code:** Click on files in the Tree View on the left to open them in a new tab in the Code Preview panel. Click folders to expand/collapse them. Use the `▸` and `▾` buttons above the file search to collapse/expand all folders.
* **Searching Files:** Use the "**Search files...**" input above the Tree View to filter the file list by name.
* **Regex Search:**
    * Enter your custom regex pattern in the "**Regex search in contents...**" input.
    * Or, select a predefined pattern from the dropdown list.
    * Click the "**Search**" button.
    * Results appear in the "**Search**" tab of the bottom panel. Click on a file path to open the file, or click on a specific code snippet to open the file and scroll to that exact line.
* **Extracting Domains:** Click the "**Domains**" button in the header. Found domains will be listed in the "**Domains**" tab of the bottom panel.
* **Code Preview Tabs:** Click tabs to switch between open files. Click the `×` on a tab to close it. Use the "**Wrap**" button to toggle word wrapping.
* **Context Menu:** Right-click on a file or folder in the Tree View for options like copying the path or downloading the individual file.

---

## Built With 🛠️

* **HTML5**
* **CSS3**
* **Vanilla JavaScript** (No external frameworks)
* **Highlight.js** - For syntax highlighting

---

## Contributing 🤝

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](LINK_TO_ISSUES_PAGE) *(<- Replace with your repo's issues link)*.

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

---

## License 📜

Distributed under the MIT License. See `LICENSE` file for more information *(<- Make sure you add an MIT LICENSE file to your repo)*.

---

## Contact 👤

Created by **Mitsec** - [@ynsmroztas](https://x.com/ynsmroztas)