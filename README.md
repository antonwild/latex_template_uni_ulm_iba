# My LaTeX Template

This LaTeX template is an almost exact (germnan) replication of the official MS Word template used for academic documents at the Institute for Business Analytics, University of Ulm. Please note that this is not an official template. I created it for use in writing my Master's thesis. It’s advisable to consult with your mentor to ensure you are permitted to use this template for your work.

## Table of Contents
1. [Installation](#installation)
2. [Usage](#usage)
3. [Included Chapters](#included-chapters)
4. [License](#license)
5. [Acknowledgments](#acknowledgments)
6. [Contact Information](#contact-information)

## Installation
I recommend using <a>https://www.overleaf.com</a> for using and editing the template
1. Download the file 'latex_template_iba'
2. Sign in to your overleaf account
3. Import the file by clicking `New Project` > `Upload Project`

## Usage
Almost every line of code is commented in englisch. Using the template should be very straight-forward. You will find several folders in the `.zip` file:
1. `layout.tex`: This `.tex` file contains the packages and settings to correctly format the document. You do not have to change anything in here to use the template correctly.
2. `images`: Upload all of your images here. Do not change the name of "iba-logo.png" and "uni-ulm-logo.png". Both logos are used in the document. 
3. `pre-chapters`: This folder holds several chapters like the declaration of the title page. You can modify the content. Do not touch the first two to three lines (`\section*{Ehrenwörtliche Erklärung}` or `\markboth{Ehrenwörtliche Erklärung}{Ehrenwörtliche Erklärung}`) unless you want to change the apperance of the document.
4. `main-content`: Add your chapters here. Every chapter with the hierarchy 1 in the table of contents should have a separate `.tex` file in this folder. Include the chapters in the `main.tex` file like so:

```latex
\input{layout} % This line imports the layout based on the `layout.tex` file
\begin{document}
\input{pre_chapter/title_page} % Import chapters from the folder `pre_chapter`
\input{main_content/introduction} % Import a chapter from the folder `main_content`. Here: 1. Introduction
\input{main_content/literature_review} % Import another chapter. Here: 2. Literature Review
\end{document}
```

4. Paste your references in the `bib.tex` format to the file `references.bib`. Personally, I like to use paperlib to store and organize scienfitic articles.

## Included Chapters
In this version, the chapters' names are german. You can easily change the name within the header of the individual `.tex` file **and** `main.tex`.

### Example
Change
```latex
\clearpage
\phantomsection
\addcontentsline{toc}{section}{KI-Tool-Verzeichnis}
\input{pre_chapter/ki-tool}
```
to
```latex
\clearpage
\phantomsection
\addcontentsline{toc}{section}{AI-Tool-Directory}
\input{pre_chapter/{ai-tool-directory}
```
### List of Chapters
- Deckblatt
- Inhaltsverzeichnis (Table of contents)
- Sperrvermerk (Confidential Clause)
- Abbildungsverzeichnis (List of figures)
- Tabellenverzeichnis (List of tables)
- Abkürzungsverzeichnis (List of Abbreviations)
- 1. Einleitung (dummy chapter)
- 2. Theoretischer Hintergrund (dummy chapter)
- Anhang (Appendix)
- Literaturverzeichnis (Bibliography)
- Ehrenwörtliche Erklärung (Declaration)
- KI-Tool-Verzeichnis (AI-Tool-Declaration)

## License
MIT License

Copyright (c) 2024 Anton Wild

Permission is hereby granted, free of charge, to any person obtaining a copy
of this template and associated documentation files (the "template"), to deal
in the template without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the template, and to permit persons to whom the template is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the template.

THE TEMPLATE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE TEMPLATE OR THE USE OR OTHER DEALINGS IN THE
TEMPLATE.


## Acknowledgments
- This template was inspired by <a>https://www.uni-ulm.de/mawi/iba/lehre/downloads/</a> (Only accessable via intranet of Uni Ulm)  

## Contact Information
For questions, please contact anton.awild@gmail.com
