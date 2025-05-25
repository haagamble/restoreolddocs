# Tajik TransCyrillicSans Word Document Restorer

This project restores Tajik text in Word documents that were originally typed using the TransCyrillicSans font. Sometimes, such text appears as Wingdings or other incorrect characters. This script replaces those with the correct Tajik Cyrillic characters using predefined mappings.

## Features

- Converts single characters and double-character pairs from TransCyrillicSans encoding to proper Tajik Cyrillic.
- Processes both regular paragraphs and tables in `.docx` files.
- Outputs a fixed document with Unicode Cyrillic text.

## Usage

1. Place the Word document you want to fix in the `docs/` folder and name it `fixme.docx`.
2. Run the script:

    ```sh
    python restore.py
    ```

3. The fixed document will be saved as `docs_fixed/fixed.docx`.

## Project Structure

- [`restore.py`](restore.py): Main script for restoring documents.
- [`subs.py`](subs.py): Contains the character and pair mappings.
- `docs/`: Place your input `.docx` files here.
- `docs_fixed/`: Output folder for fixed documents.

## Requirements

- Python 3.x
- [`python-docx`](https://python-docx.readthedocs.io/en/latest/)

Install dependencies with:

```sh
pip install python-docx
```

## Customization

- To process a different file, change the input/output paths in [`restore.py`](restore.py).
- You can modify or extend the mappings in [`subs.py`](subs.py) as needed.

