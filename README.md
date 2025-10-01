# Automatic-File-Sorter

This project is a Python script that automates file organization within a given folder.  

It uses the built-in `os` and `shutil` libraries to scan files, create categorized folders, and move files based on their extensions.



## How It Works

1. The program scans all files inside a target directory.  

2. A dictionary defines how file extensions should be grouped. Example:

&nbsp;  file\_types = {

&nbsp;      "jpg": "Image Files",

&nbsp;      "png": "Image Files",

&nbsp;      "csv": "CSV Files",

&nbsp;      "txt": "Text Files"

&nbsp;  }



3. The script creates the necessary folders inside the directory (e.g., Image Files, CSV Files, Text Files).

4. Each file is checked for its extension:
- If the extension matches the dictionary, the file is moved into the corresponding folder.
- If the extension is not in the dictionary, the file remains in place.



## Example
### Before running the script:

/Downloads

&nbsp;  ├── report.csv

&nbsp;  ├── notes.txt

&nbsp;  ├── photo.jpg

&nbsp;  ├── graphic.png

### After running the script:

/Downloads

&nbsp;  ├── CSV Files

&nbsp;  │    └── report.csv

&nbsp;  ├── Text Files

&nbsp;  │    └── notes.txt

&nbsp;  └── Image Files

&nbsp;       ├── photo.jpg

&nbsp;       └── graphic.png


##Purpose
This project demonstrates how to use Python for file automation and organization, showcasing skills in working with the filesystem, dictionaries, and conditional logic.
It is also part of my portfolio, illustrating practical problem-solving with Python.