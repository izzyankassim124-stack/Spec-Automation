# JAXER – Auto Format Jadual Spesifikasi

A static, browser-based tool for formatting tender specification data into an Excel workbook.


## How the tool works

- Paste a table copied from ePerolehan, or upload an `.xlsx` file.
- Choose the header and item-row colours.
- Generate and download the formatted `.xlsx` workbook.
- Data processing is performed in each user's browser. This static page does not upload the pasted data or selected workbook to a server, and it does not provide a shared database or Synology integration.

## Dependency and network requirement

The page loads ExcelJS 4.4.0 from jsDelivr:
`https://cdn.jsdelivr.net/npm/exceljs@4.4.0/dist/exceljs.min.js`

Users need internet access to load this library. If the office network blocks jsDelivr, the Excel generation feature may not work until the library is hosted locally or the network allows it. Google Fonts are optional; fallback fonts are included.

## Updating the website

Edit `index.html`, upload the updated file to the same repository, and commit the change. GitHub Pages will redeploy automatically from the `main` branch root.
