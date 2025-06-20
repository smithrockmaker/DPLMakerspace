## Operator Notes:

As part of creating this book there are a bunch of new processes that I've had to get comfortable with. Here is the documentation for those steps for future reference. The primary reference I have used, with  lots of help from other sources, is the [Jupyterbook tutorial](https://jupyterbook.org/start/your-first-book.html).

### jbook Environment:

I'm still need reminders in this environment but am realizing that creating a few separate environments for projects that need distinct software packages reduces the opportunities for conflicts between the different packages. 

The initial step is to start Jupyterlab from the jbook environment in Anaconda. This apparently connects all the paths appropriately this collection of software packages. **Note:** Ben R notes that he now works entirely in python and never uses Jupyterlab but I still think connecting the documentation and coding in one notebook is the best mode for me. Just noting....

In the terminal window the prompt will indicate the active environment and even if I open Jupyterlab from the jbook environment the (base) environment will be where the terminal lands. The prompt will look something like this.

```
(base) bruceemerson@Bruces-MacBook-Pro ~ %
```

When starting to work on the book activate the jbook environment using ``` conda activate jbook```.
```
(base) bruceemerson@Bruces-MacBook-Pro ~ % conda activate jbook
```
After doing so the prompt will indicate the jbook environment.
```
(jbook) bruceemerson@Bruces-MacBook-Pro book % 
```

### Navigate to root directory:

The next step is to navigate to the root directory for the book. This is the directory which contains the \_toc.yml file as well as the\_build folder where the built book is stored. Navigate using the usual 'cd', 'ls', and 'pwd' unix tools to navigate. Here is the ultimate destination for the Barca22 book.
```
/Users/bruceemerson/Documents/Jupyter/JupyterLabRepos/3DPrinterBasics
```
### Build the book:

The book is built locally with the 'jupyterbook build' using the 'jb' shorthand. jupyterbook has a number of expectations about the nesting of markdown language and I usually get lots of red violations
```
(jbook) bruceemerson@Bruces-MacBook-Pro book % jb build .
```
jupyterbook has a number of expectations about the nesting of markdown language and I usually get lots of red violations like the following but they don't seem to keep the book from being built.
```
/Users/bruceemerson/Documents/Jupyter/JupyterLabRepos/Barca22/book/barcaSAE/Schedule.md:1: WARNING: Non-consecutive header level increase; 0 to 2 [myst.header]
```
This is the happy message I hope to get at the end of the build process.
```
===============================================================================

Finished generating HTML for book.
Your book's HTML pages are here:
    _build/html/
You can look at your book by opening this file in a browser:
    _build/html/index.html
Or paste this line directly into your browser bar:
    file:///Users/bruceemerson/Documents/Jupyter/JupyterLabRepos/Barca22/book/_build/html/index.html            

===============================================================================
```

### Public Book

I plan for this 'book' to be public but I'm not sure all that that will entail. 
