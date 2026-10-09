.PHONY: all clean

all:
	latexmk -pdf -interaction=nonstopmode -halt-on-error -file-line-error -outdir=.build resume_work.tex
	cp .build/resume_work.pdf ../Akmal_Ashirmatov_CV.pdf

clean:
	latexmk -C -outdir=.build resume_work.tex
