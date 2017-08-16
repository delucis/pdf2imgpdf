# pdf2imgpdf

A command line utility that converts a PDF into a PDF! 😲 🎉

Each page of the source PDF is converted to a PNG image, then these are
recombined into a PDF.


## Installation

```sh
brew install delucis/tap/pdf2imgpdf
```


## Usage

```
Usage:
  pdf2imgpdf [options ...] file|directory

Options:
  -h                display this help message
  -o directory      the name of the directory to save your ouput PDFs to (default: img-pdfs)
  -p prefix         a prefix to add to the filename of your output PDFs
  -r resolution     image resolution, in DPI (default: 150)
  -s suffix         a suffix to add to the filename of your output PDFs
  -v                print the current version number to the Terminal window

Examples:
  Process all the PDFs in the directory 'old-pdfs', saving them to the directory 'new-pdfs'
  with the prefix 'Copy of ' in front of their original file name:

        pdf2imgpdf -o new-pdfs -p "Copy of " old-pdfs


  Process 'my-document.pdf', saving it to the current directory with the suffix '-processed':

        pdf2imgpdf -o . -s -processed my-document.pdf


  Create a very low resolution, pixelated copy of 'my-document.pdf':

        pdf2imgpdf -r 10 my-document.pdf


```
