# ATS Resume Builder

A free, guided resume builder for students. Answer 13 short steps and download a one-page, ATS-safe resume as PDF or Word.

Everything runs in your browser: no sign-up, no API key, no usage limit.

**Live site:** _link coming after the first deploy_

## What it does

- **Guided 13-step form**: contact details, links, target role, education, languages, tools, up to three projects, certifications, achievements and work experience.
- **Bullet coach**: checks every bullet as you type for an action verb, a real number, and a length that fits on two lines.
- **Bullet helper**: pick a verb, describe what you did and the result, and it writes the bullet for you.
- **Summary generator**: writes a two to three sentence summary from your answers. You can edit it.
- **Role keyword check**: compares your resume with common keywords for 8 fresher roles (software, full stack, data analyst, data science/ML, cybersecurity, cloud/DevOps, IT support, product/project management).
- **Fix before applying**: a checklist of specific problems, such as missing links, bullets without numbers, or a phone number without a country code.
- **Certification roadmap**: 18 certifications, checked on 30 September 2026, with free options first. Ones you already hold are skipped.
- **ATS view**: shows the plain text a resume parser reads from your PDF.
- **Exports**: a text-based A4 PDF in a single column, and an editable Word (.docx) file, named `Firstname-Lastname-Resume`.

## Privacy

Nothing you type is uploaded. Your answers are saved in your own browser (localStorage), and **Start over** deletes them. The only outside requests are Google Fonts, plus the jsPDF library from jsDelivr, which loads when you download a PDF.

## Run it locally

It is a single file. Download `index.html` and open it in any browser. The PDF download needs an internet connection the first time, to load jsPDF.

## Host your own copy

Fork this repository, then either:

- import it on [Vercel](https://vercel.com/new) (framework preset: Other, no build command), or
- turn on GitHub Pages (Settings, then Pages, deploying from the `main` branch).

## Tech

Plain HTML, CSS and JavaScript in one file, with no build step. PDF export uses [jsPDF](https://github.com/parallax/jsPDF). The Word file is written directly as Office Open XML inside a small zip writer.

## Keeping it accurate

Certification offers and exam prices change. If you spot something out of date or a broken link, please open an issue.

Made by Shivam Pandey.
