PDF = pdflatex
PDFFLAGS =
AUX = ./.aux

informe: informe.pdf 

informe.pdf: informe.tex
	mkdir -p .aux
	$(PDF) $(PDFFLAGS) -output-directory $(AUX) -jobname=informe informe.tex 
	mv $(AUX)/$@ .

clean : .PHONY
	rm -fr $(AUX)
.PHONY :
