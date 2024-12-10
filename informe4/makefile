PDF = pdflatex
PDFFLAGS =
AUX = ./.aux
DEPS = ./content/1-intro.tex ./content/2-diseño.tex ./content/3-conclusiones.tex ./content.tex ./titlepage.tex ./content/img/mvc.png ./logo.png

#informe: informe.pdf $(DEPS)

informe.pdf: informe.tex $(DEPS)
	mkdir -p .aux
	$(PDF) $(PDFFLAGS) -output-directory $(AUX) -jobname=informe informe.tex 
	$(PDF) $(PDFFLAGS) -output-directory $(AUX) -jobname=informe informe.tex 
	mv $(AUX)/$@ .

clean : .PHONY
	rm -fr $(AUX)
	rm *.aux *.fdb_latexmk *.fls *.lof *.log *.lot *.out  *.toc

.PHONY :
