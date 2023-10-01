ps_source := presentation.tex
rp_source := report.tex
ps_deps := $(wildcard ps_*.tex)
rp_deps := $(wildcard rp_*.tex)

presentation: $(ps_source) $(ps_deps)
	lualatex -shell-escape $(ps_source)

report: $(rp_source) $(rp_deps)
	lualatex -shell-escape $(rp_source)

all: presentation report

clean:
	rm -f *.pdf *.aux *.log *.out *.nav *.toc *.snm
