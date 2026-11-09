# CppForge — Online C++ Compiler

A lightweight browser-based C++ playground for learning and competitive programming.

## Features
- C++ editor with syntax highlighting, line numbers, bracket matching, and indentation (CodeMirror 5).
- Run C++ code remotely using GCC through the Piston API.
- Uses the GCC 10.2.0 runtime provided by Piston.
- Custom standard input and separate output / compiler diagnostics.
- Quick snippets for common algorithms and STL patterns.
- STL pocket reference for commonly used containers and functions.
- Responsive layout for desktop and mobile.

## Run locally
Open `index.html` in a modern browser. An internet connection is required for the editor CDN assets and remote compilation.

## Deploy with GitHub Pages
1. Open **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select your default branch and the `/(root)` folder, then save.
4. Wait for the Pages deployment to finish. Your site URL will be shown in the Pages section.

## How compilation works
When you click **Run code**, the browser sends the source code and standard input to the public Piston API, which compiles and runs it using GCC. The app does not run a compiler locally. Avoid entering secrets into the editor.

## Notes
- The remote execution service has its own rate limits, compiler version, and execution limits.
- C++ standard selection is sent as a compiler preference; the available compiler version is controlled by the execution service.
