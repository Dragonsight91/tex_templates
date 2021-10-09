# LaTeX Email 
## NOTE
This may not work with all mail clients. So far, i know that Thunderbird does support this, but Gmail does not

## Prerequisites

- [`pdf2htmlEX`](https://github.com/pdf2htmlEX/pdf2htmlEX) to convert the PDF to HTML
- [`thunderbird`](https://www.thunderbird.net/en-US/) to send an email 
- [`stationery`](https://addons.thunderbird.net/en-US/thunderbird/addon/stationery/) to be able to directly edit the HTML (and essentially copy-paste the output HTML)

## How to use?
Here's how to do it on linux, assuming latex is set up
1. compile the LaTeX PDF with your favorite recipe
2. convert the PDF to HTML with `pdf2htmlEX --embed "cCfFiIjJoO" path/to/file.pdf` the `--embed "cCfFiIjJoO"` makes sure that all fonts, images and styles are embedded into the HTML, so that you don't need to worry about missing fonts on the recipients PC
3. (assuming your [email account is added to thunderbird](https://www.lclark.edu/live/files/3166)) Install the [Stationery Addon](https://support.mozilla.org/en-US/kb/installing-addon-thunderbird)
4. create an email
5. switch to the `HTML` tab
6. Delete all existing HTML
7. copy the HTML text from the HTML file and paste it into the email
8. switch back to the `edit` tab and check the layout and style.
9. if all is okay, send it
