Overview
This Python script automates the mapping process between hospital items and manufacturer SKUs for a Request for Quotation (RFQ) project. It reads hospital baseline data and manufacturer consolidated data, then categorizes items into "Mapped" (matched with hospital items) and "Not Mapped" sheets.

Features
Reads hospital and manufacturer Excel files with flexible column detection.

Matches manufacturer SKUs with hospital MFS identifiers.

Generates separate output Excel files per manufacturer:

Mapped Sheet: Items with matching hospital MFS.

Not Mapped SKUs: Items not present in hospital baseline.

Applies Excel styling for readability including color fills, borders, and column auto-sizing.

Leaves cost fields blank for user input as per requirements.

Dynamically creates an index sheet explaining column definitions and purpose.

Supports batch processing of all manufacturers in the consolidated manufacturer file.

Outputs saved in a configurable output directory.

Usage
Place your hospital baseline Excel file and consolidated manufacturer Excel file in accessible paths.

Configure the hospital_file, manufacturers_file, and output_folder variables in the script.

Run the script in a Python environment with dependencies: pandas, openpyxl.

Check the output folder for manufacturer-specific Excel files with mapped and not mapped sheets.

Dependencies
pandas

openpyxl

File Details
Input: Hospital mapping baseline Excel file.

Input: Consolidated manufacturer SKUs Excel file.

Output: Manufacturer-wise Excel files with "Mapped" and "Not Mapped SKUs" sheets.
