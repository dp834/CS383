

PYTHON_NOTEBOOK = Homework3.ipynb

IMG_OUTPUT = images/

LATEX_SRC  = Homework-3.tex
PDF_OUTPUT = Homework-3

run: $(PYTHON_NOTEBOOK)
	mkdir -p $(IMG_OUTPUT)
	ipython3 $(PYTHON_NOTEBOOK)

pdf: $(LATEX_SRC)
	pdflatex -jobname $(PDF_OUTPUT) $(LATEX_SRC)

clean:
	@rm -rf $(IMG_OUTPUT)/ $(PDF_OUTPUT).pdf *.aux *.log &2> /dev/null || true
