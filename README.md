# Documentation and Training Materials for the **PacSAFE Project**

Enhancing the ability of disaster managers in the Pacific region to prepare for and respond to disasters, and to reduce the impacts of disasters on the local population and infrastructure.

### Requirements:

* `Sphinx` v1.4.8 or later
* `sphinx_rtd_theme` v0.2.4 or later

### General guidelines:

The intention is to maintain materials for individual workshops in separate sub-directories. This is because the PacSAFE training material is tailored to the country audience, because the scenarios packaged with the application are tailored to each country.

Currently images are stored in a single folder at the top level. This presently is easiest to manage, but as additional workshops are compiled, it is likely we'll need to create a sub-directory structure similar to the source files. 



### To build the HTML pages locally:

Simply run `make html` in the parent directory. This will build the html pages under `_build/html`. Opening the `index.html` file will open the page in a browser window and allow you to navigate the complete documentation for PacSAFE.


### To build separate PDF doc for training workshop:

1. Try to avoid using image files like .ico, or the generic .* directive in the RST files. 
2. copy the /images folder to the training workshop directory
3. copy Makefile, make.bat and conf.py to the same directory
4. Run `make latex` to generate the latex file. The output will be created in `_build/latex`
5. Use TeXworks or another latex compiler to build the PDF (should be pacsafe-doc.tex).
6. Move the completed PDF file somewhere safe (called pacsafe-doc.pdf)
7. Run `make clean` to clear the _build directory
8. Remove the /images subdirectory, and the Makefile, make.bat, conf.py


---

Ⓒ 2017 -  GA, SPC

Community Safety and Earth Monitoring Division, Geoscience Australia (GA)
Geoscience Division, Pacific Commuity (SPC)

