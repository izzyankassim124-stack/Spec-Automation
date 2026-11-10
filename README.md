# JAXER – Auto Format Jadual Spesifikasi

A static, browser-based tool for formatting tender specification data into an Excel workbook.

## Publish with GitHub Pages (GitHub Free)

> Important: On GitHub Free, the repository must be **Public** to use GitHub Pages. The published website is publicly accessible to anyone with the URL, and the repository source code is visible too. Do not put confidential tender documents, company data, passwords, API keys, or other secrets in this repository.

1. Sign in to https://github.com/.
2. Create a new repository, for example `jaxer-auto-format`.
3. Set repository visibility to **Public** and create the repository.
4. Extract this ZIP file on your computer.
5. In the new GitHub repository, choose **Add file → Upload files**.
6. Upload `index.html` (and this `README.md` if desired) to the repository's top level. The file must be named exactly `index.html`.
7. Click **Commit changes**.
8. Open **Settings → Pages** in the repository.
9. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
10. Select branch **main** and folder **/(root)**, then click **Save**.
11. Open the **Actions** tab and wait for the Pages deployment workflow to finish successfully.
12. Return to **Settings → Pages**. Use **Visit site**. The URL will look like `https://YOUR-GITHUB-USERNAME.github.io/jaxer-auto-format/`.
13. Share that URL with colleagues and test it on another office laptop.

GitHub Pages may take several minutes to publish after the first setup or after a change.

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

## Privacy and limitations

- GitHub Pages is public hosting; it is not an access-controlled company portal.
- Do not publish confidential JAXER data or documents.
- Each colleague uses the tool independently in their own browser and downloads their own output.
- This tool does not log in employees, save shared tender records, update task statuses, or connect to Synology.
