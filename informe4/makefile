PDF = pdflatex
PDFFLAGS =
AUX = ./.aux
DEPS = ./content/1-intro.tex ./content/2-diseño.tex ./content/3-conclusiones.tex ./content.tex ./titlepage.tex ./content/img/MVC.png ./logo.png ./content/img/Crear_alarma_intervalos.png ./content/img/Crear_Alarma_Unica.png ./content/img/Desactivar_alarma.png ./content/img/Desafio_Aritmetico.png ./content/img/Desafio_Memorice.png ./content/img/Desafio_Rompecabezas.png ./content/img/Eliminar_Alarma_Intervalos.png ./content/img/Eliminar_Alarma_Unica.png ./content/img/Modificar_Alarma_Intervalos.png ./content/img/Modificar_Alarma_Unica.png

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
