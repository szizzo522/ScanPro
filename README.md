# ScanPro File Scanner:
ScanPro is a Python-based GUI application that monitors your Downloads folder for new files and scans them for potential risks. Watchdog is a Python library that monitors file system events. It allows programs to detect when files and directories are created, modified, moved, or deleted. The app compares the file’s extension (for example, .exe, .js, .bat) against a list of extensions known to be associated with executable or potentially dangerous files. If it finds a match, it flags the file as high risk. It also uses Python’s mimetypes module to guess the file’s type. While this doesn’t tell you everything about the file’s content, it helps verify if the file’s nature (like being an application or script) aligns with its extension. Based on these checks, the app then outputs a risk level (“HIGH” for risky extensions, “LOW” otherwise) along with a recommendation on whether it’s safe to open the file.

## Features:
- Monitors the Downloads folder for new files.
- Scans files for size, type, and potentially risky extensions.
- Allows manual file scanning.
- Displays results in a user-friendly GUI.

## Requirements:
- python version 3.8 or later
- watchdog

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
python3 Scanpro.py

## License
Copyright (c) 2025 Samuel Zizzo

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

This license applies to the ScanPro project.

## Comments
***This was created using python version 3.12.2***

***This is a basic scanner—it doesn’t actually analyze the file’s internal code or behavior. More advanced scanners use signature-based or heuristic analysis, sometimes even running files in a sandbox. This version is meant as a learning tool and a simple first line of defense.***
