# Portfolio Website

Personal portfolio website for Wonji Seo, Product Manager.

## Project Structure

- `index.html`: Main landing page.
- `portfolio.html`: Portfolio page (currently mirrors index).
- `projects.json`: Data for the Side Projects section.
- `blog.json`: Data for the Blog Posts section.
- `design.md`: Design system and guidelines.

## Data Management

The content for "Side Projects" and "Blog Posts" is managed via a Google Spreadsheet.
Updates to the spreadsheet should be exported to the respective JSON files (`projects.json` and `blog.json`) in this repository.

[**View Data Spreadsheet**](https://docs.google.com/spreadsheets/d/1eRcZ4n_uSj2SREyyYrbFguv43-jYWQRAGcu-b7RTTnY/edit?gid=1928574215#gid=1928574215)

## Development

To view the site locally:
1. Clone the repository.
2. Open `index.html` in your browser.
   - **Note**: Dynamic content loading (JSON fetch) works best when running a local server (e.g., `python3 -m http.server` or VS Code Live Server) to avoid CORS issues. Fallback data is included in the script for direct file opening explanation.
