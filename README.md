Digital Forensics – File Metadata Extraction Tool

A Python-based digital forensics utility designed to extract and display file-system metadata. This project demonstrates fundamental digital forensic concepts through file inspection, metadata extraction and timestamp analysis.

Project Overview

This project implements a simple file metadata extraction tool using Python.

The application prompts the user to provide a file or directory path, verifies whether the path exists, and extracts relevant file-system metadata.

The extracted information is presented in a structured, readable format.

Features
File and directory existence verification.
File and directory name extraction.
Absolute path identification.
File size extraction in bytes.
File timestamp extraction.
Last-modified timestamp identification.
File type identification.
Basic error handling for non-existent paths.
Technologies Used
Python 3 – Primary programming language.
Pathlib – File-system path handling and metadata access.
Datetime – Timestamp conversion and formatting.
Pprint – Structured output formatting.

All dependencies are included in Python's standard library.

Project Structure
digital-forensics-file-metadata/
│
├── forensics.py
│
└── README.md
Requirements
Python 3.8 or later.
Access to the file or directory being examined.
Installation and Usage

1. Clone the repository

git clone https://github.com/Cameron007-D/digital-forensics-file-metadata.git

2. Navigate into the project directory

cd digital-forensics-file-metadata

3. Run the Python script

python forensics.py

On Linux, you may need:

python3 forensics.py

4. Enter the full file path when prompted.

Example:

Enter the full path to the file: C:\Users\YourName\Documents\example.pdf

The application will display the extracted metadata.

Metadata Collected
Metadata	Description
File Name	Name of the examined file or directory
Absolute Path	Full resolved file-system path
File Size	File-system size in bytes
Created On	Timestamp derived from st_ctime
Last Modified	Timestamp derived from st_mtime
File Type	Identifies whether the path is a file or directory
Digital Forensics Considerations

The interpretation of file-system timestamps depends on the operating system.

On Windows, st_ctime generally represents the file creation time. On Linux and other Unix-like systems, it generally represents the last metadata or status change time rather than the original creation time.

File-system metadata can also be affected by copying, moving or modifying files.

This project is an educational demonstration of introductory digital forensics concepts. It is not intended to replace professional forensic acquisition, evidence preservation or validation procedures.

Future Improvements
Implement MD5 and SHA-256 file hashing.
Introduce JSON and CSV metadata reporting.
Expand file permission analysis.
Improve exception handling.
Implement automated unit testing.
Author

Cameron Davhana

GitHub: Cameron007-D

Developed as part of my Digital Forensics and Cybersecurity learning journey.
