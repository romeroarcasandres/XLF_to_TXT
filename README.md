# XLF_to_TXT

This script converts .xlf and .po files to .txt/.xlsx format, extracting the source and target texts into two tab-separated columns.

## Overview

The `XLF_to_TXT` script processes XLIFF files, parsing the XML tags <source> and <target> to extract source and target language texts. It then writes these texts to a tab-separated .txt file and an Excel file (.xlsx), preserving the language information and ensuring that each line corresponds to a translation unit from the XLIFF file.
It’s compatible with all XLIFF formats: .sdlxliff, mqxliff, mxliff.
It also processes PO files.

## Requirements

- Python 3
- `xml.etree.ElementTree` library (for XML parsing)
- `pandas` library (for data manipulation and exporting to .txt)
- `tkinter` library (for file dialog)
- `os` library (for file path operations)
- `re` library (for regular expressions)

## Files

- `XLF_to_TXT.py`

## Usage

1. Run the script.
2. A file dialog will prompt you to select the file.
3. After selecting the file, the script will parse its content and extract the source and target texts.
4. The resulting .txt & .xlsx files will be saved in the same directory as the selected XLIFF file with the same name but with a ".txt" or ".xlsx" extension.

## Important Note

Ensure that the selected file is a valid XLIFF file.
The script assumes the XLIFF file follows standard structure with <source> and <target> tags.
Tags within the extracted texts are removed for the output to be only plain text in the .txt file.

## License
This project is governed by the GNU Affero General Public License v3.0. For comprehensive details, kindly refer to the LICENSE file included with this project.
