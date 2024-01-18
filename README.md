# Thesis_LaTeX_Template
Template provided by SFSU Mathematics department.

## Audience for this
Someone new to LaTeX like I was when starting my thesis work. For questions, please don't hesitate to reach out. I am not an expert, but I have gained a lot of experience searching for the correct answer and using trial/error to solve problems I encountered. 

## Notes on TeX files
There is only one file that needs to be run in this folder to produce a pdf of the entire thesis: thesis.tex. If you run the other files, you will encounter an error. If you want to see how just one part of the overall thesis looks, comment out the other parts. For example, if you only want to see the introduction then you would use the % symbol at the beginning of the lines for all the other parts of the thesis. Then run pdfLaTeX. 

The other .tex files should be filled in with the relevant information. For example, abstract.tex should include a brief summary of the work presented in your thesis. 

To include figures in the document

## Notes on Citations
Other than the .tex files (sorting by file type will help you identify these), the only other file to edit is the references file which is a BibTeX Database type file. Google Scholar is a great resource for acquiring this citation type for all of your references. When searching for a reference using Google Scholar, make sure that the "include citations" box (lefthand side of screen) is checked. Under each entry you can access the BibTeX citation by clicking on "Cite". Then choose "BibTeX" and copy/paste. This method will ensure you have the proper formatting for each source you used. (To avoid plagiarism accusations like those in the news recently, make sure to cite absolutely every source used.)

## Potential Issues
When running the the thesis.tex file, I ran into a problem with my citations not rendering properly (they stayed in the LaTeX format of \cite{} and the bibliography did not populate). Since thesis.tex has "\usepackage{biblatex}", running the file using BibTeX will not work. The fix for this requires running the thesis.tex file three times: first with pdfLaTeX, then with Biber (which handles the citations properly), then lastly with pdfLaTeX again. 

This is a valuable resource for other issues: https://www.latex-project.org/help/
