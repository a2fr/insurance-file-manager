# Insurance File Manager

A Windows desktop application for centralising day-to-day insurance operations: client records, contracts, documents, payments, and cancellations.

## Problem addressed

Insurance administration often spreads client information across folders, documents, and spreadsheets. This prototype brings the main workflows into one interface while preserving compatibility with an existing file- and Excel-based organisation.

## Main workflows

- Create and search client records
- Add and manage insurance contracts
- Organise client and contract documents
- Record and search payments
- Merge client folders
- Process contract cancellations
- Open the active client directory from the application

## Technical choices

- **Electron and Node.js** provide a desktop UI with local file-system access.
- **IPC events** connect the HTML interface to the main application process.
- **Excel workbooks** act as a lightweight data store through `xlsx` and `exceljs`.
- **File-system integration** keeps business documents organised in client directories.

## Tech stack

Electron · Node.js · JavaScript · HTML/CSS · xlsx · exceljs

## Current status

This repository is a functional prototype. Its workbook and directory paths are tailored to the original Windows environment and must be configured before it can run elsewhere. No real client data is included.

To run it locally, install the dependencies with `npm install`, configure the paths in `main.js`, and start the application with `npm start`.
