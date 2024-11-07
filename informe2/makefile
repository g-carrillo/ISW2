PDF = pdflatex
PDFFLAGS =
AUX = ./.aux
	DEPS = ./content/1-intro.tex ./content/2-requerimientos.tex ./content/3-casos.tex ./content/4-conclusiones.tex ./content.tex ./titlepage.tex

#informe: informe.pdf $(DEPS)

informe.pdf: informe.tex $(DEPS)
	mkdir -p .aux
	$(PDF) $(PDFFLAGS) -output-directory $(AUX) -jobname=informe informe.tex 
	$(PDF) $(PDFFLAGS) -output-directory $(AUX) -jobname=informe informe.tex 
	mv $(AUX)/$@ .

clean : .PHONY
	rm -fr $(AUX)
.PHONY :
