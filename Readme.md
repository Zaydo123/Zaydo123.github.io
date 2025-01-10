# Resume Project

This project is a personal resume website created using HTML and CSS. The website showcases my professional experience, education, skills, and projects. It includes the following features:

- **Resume Display**: The main page (`index.html`) displays my resume in a well-structured format. It includes sections for education, experience, extracurricular involvement, projects, and skills.
- **PDF Download**: A button on the main page allows users to download the resume as a PDF file. This functionality is powered by a GitHub Action that converts the HTML resume to a PDF format.
- **Last Updated Date**: The website dynamically displays the last updated date of the resume, which is fetched from a text file (`public/date.txt`).

## How It Works

1. **HTML to PDF Conversion**: The GitHub Actions workflow (`html-to-pdf.yml`) runs on every push or pull request to the master branch. It uses the `fifsky/html-to-pdf-action` to convert `index.html` to `resume.pdf`.
2. **Updating Last Modified Date**: The workflow also updates the `public/date.txt` file with the current date, which is then displayed on the website.
