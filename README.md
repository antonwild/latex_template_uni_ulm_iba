# My LaTeX Template

This LaTeX template is an almost exact replication of the official MS Word template used for academic documents at the Institute for Business Analytics, University of Ulm. Please note that this is not an official template. I created it for use in writing my Master's thesis. It’s advisable to consult with your mentor to ensure you are permitted to use this template for your work.

## Table of Contents
1. [Installation](#installation)
2. [Usage](#usage)
3. [Included Chapters](#included-chapters)
4. [Contributing](#contributing)
5. [License](#license)
6. [Acknowledgments](#acknowledgments)
7. [Contact Information](#contact-information)

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
\input{layout}
\begin{document}
\input{pre_chapter/title_page} 
\input{main_content/introduction}
\input{main_content/literature_review}
\end{document}
```

4. Paste your references in the `bib.tex` format to the file `references.bib`. Personally, I like to use paperlib to store and organize scienfitic articles.

## Included Chapters

## Acknowledgments
- This template was inspired by <a>https://www.uni-ulm.de/mawi/iba/lehre/downloads/</a> (Only accessable via the university connection)  

## Contact Information
For questions, please contact anton.awild@gmail.com
