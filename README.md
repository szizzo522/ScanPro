# ScanPro File Scanner:python
ScanPro is a Python-based GUI application that monitors your Downloads folder for new files and scans them for potential risks. Watchdog is a Python library that monitors file system events. It allows programs to detect when files and directories are created, modified, moved, or deleted. The app compares the file’s extension (for example, .exe, .js, .bat) against a list of extensions known to be associated with executable or potentially dangerous files. If it finds a match, it flags the file as high risk. It also uses Python’s mimetypes module to guess the file’s type. While this doesn’t tell you everything about the file’s content, it helps verify if the file’s nature (like being an application or script) aligns with its extension. Based on these checks, the app then outputs a risk level (“HIGH” for risky extensions, “LOW” otherwise) along with a recommendation on whether it’s safe to open the file.

## Features:
- Monitors the Downloads folder for new files.
- Scans files for size, type, and potentially risky extensions.
- Allows manual file scanning.
- Displays results in a user-friendly GUI.

## Requirements:
- 'python' version 3.8 or later
- 'tkinter'
- 'watchdog'

## Installation
1. Clone repository:
   '''bash
   git clone https://github.com/your-szizzo522/ScanPro.git
2. Install dependencies:
   ```bash
   pip install -r requirements.txt

## Usage
- Run the script:
   ```bash
   python Scanpro.py

## License
MIT License

## Comments
*This was created using python version 3.12.2

**This is a basic scanner—it doesn’t actually analyze the file’s internal code or behavior. More advanced scanners use signature-based or heuristic analysis, sometimes even running files in a sandbox. This version is meant as a learning tool and a simple first line of defense.