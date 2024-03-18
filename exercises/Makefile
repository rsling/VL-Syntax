# Roland's Make system for LaTeX.

# Compile system.
LX = xelatex

# Project name and file name parts.
PROJECT = SchaeferSyntaxUebungen
OUTDIR = output

# TeX Sources to watch.
SOURCEDIR = includes/
SOURCES = main.tex $(wildcard $(SOURCEDIR)/*.tex)

# Stuff passed to XeLaTeX.
MAININCLUDE = \input{main}
MULOE=\def\SOLUTIONS{}

# XeLaTeX flags.
TEXFLAGS = -output-directory=$(OUTDIR)

INPUT02=\def\LEKTION{02}\def\TITLE{02 | Kongruenz, Rektion, Valenz}\input{uebung.tex}
INPUT04=\def\LEKTION{04}\def\TITLE{04 | Phrasen und Satzglieder}\input{uebung.tex}
INPUT05=\def\LEKTION{05}\def\TITLE{05 | Nominalphrasen}\input{uebung.tex}
INPUT06=\def\LEKTION{06}\def\TITLE{06 | Weitere Phrasentypen}\input{uebung.tex}
INPUT07=\def\LEKTION{07}\def\TITLE{07 | Verbphrasen und Verbkomplexe}\input{uebung.tex}
INPUT08=\def\LEKTION{08}\def\TITLE{08 | Sätze}\input{uebung.tex}
INPUT09=\def\LEKTION{09}\def\TITLE{09 | Nebensätze}\input{uebung.tex}
INPUT10=\def\LEKTION{10}\def\TITLE{10 | Subjekte und Prädikate}\input{uebung.tex}

# Create output dir if needed.
$(info $(shell [ ! -d $(OUTDIR) ] && mkdir -p ./$(OUTDIR)/includes))


# Phony shit.

.PHONY: uebung02 uebung04 uebung05 uebung06 uebung07 uebung08 uebung09 uebung10 muloe02 muloe04 muloe05 muloe06 muloe07 muloe08 muloe09 muloe10 all

uebung02:
	$(LX) -no-pdf -jobname=$(PROJECT)02 $(TEXFLAGS) "$(INPUT02)"
	$(LX) -jobname=$(PROJECT)02 $(TEXFLAGS) "$(INPUT02)"

uebung04:
	$(LX) -no-pdf -jobname=$(PROJECT)04 $(TEXFLAGS) "$(INPUT04)"
	$(LX) -jobname=$(PROJECT)04 $(TEXFLAGS) "$(INPUT04)"

uebung05:
	$(LX) -no-pdf -jobname=$(PROJECT)05 $(TEXFLAGS) "$(INPUT05)"
	$(LX) -jobname=$(PROJECT)05 $(TEXFLAGS) "$(INPUT05)"

uebung06:
	$(LX) -no-pdf -jobname=$(PROJECT)06 $(TEXFLAGS) "$(INPUT06)"
	$(LX) -jobname=$(PROJECT)06 $(TEXFLAGS) "$(INPUT06)"

uebung07:
	$(LX) -no-pdf -jobname=$(PROJECT)07 $(TEXFLAGS) "$(INPUT07)"
	$(LX) -jobname=$(PROJECT)07 $(TEXFLAGS) "$(INPUT07)"

uebung08:
	$(LX) -no-pdf -jobname=$(PROJECT)08 $(TEXFLAGS) "$(INPUT08)"
	$(LX) -jobname=$(PROJECT)08 $(TEXFLAGS) "$(INPUT08)"

uebung09:
	$(LX) -no-pdf -jobname=$(PROJECT)09 $(TEXFLAGS) "$(INPUT09)"
	$(LX) -jobname=$(PROJECT)09 $(TEXFLAGS) "$(INPUT09)"

uebung10:
	$(LX) -no-pdf -jobname=$(PROJECT)10 $(TEXFLAGS) "$(INPUT10)"
	$(LX) -jobname=$(PROJECT)10 $(TEXFLAGS) "$(INPUT10)"


muloe02:
	$(LX) -no-pdf -jobname=$(PROJECT)02Muloe $(TEXFLAGS) "$(MULOE)$(INPUT02)"
	$(LX) -jobname=$(PROJECT)02Muloe $(TEXFLAGS) "$(MULOE)$(INPUT02)"

muloe04:
	$(LX) -no-pdf -jobname=$(PROJECT)04Muloe $(TEXFLAGS) "$(MULOE)$(INPUT04)"
	$(LX) -jobname=$(PROJECT)04Muloe $(TEXFLAGS) "$(MULOE)$(INPUT04)"

muloe05:
	$(LX) -no-pdf -jobname=$(PROJECT)05Muloe $(TEXFLAGS) "$(MULOE)$(INPUT05)"
	$(LX) -jobname=$(PROJECT)05Muloe $(TEXFLAGS) "$(MULOE)$(INPUT05)"

muloe06:
	$(LX) -no-pdf -jobname=$(PROJECT)06Muloe $(TEXFLAGS) "$(MULOE)$(INPUT06)"
	$(LX) -jobname=$(PROJECT)06Muloe $(TEXFLAGS) "$(MULOE)$(INPUT06)"

muloe07:
	$(LX) -no-pdf -jobname=$(PROJECT)07Muloe $(TEXFLAGS) "$(MULOE)$(INPUT07)"
	$(LX) -jobname=$(PROJECT)07Muloe $(TEXFLAGS) "$(MULOE)$(INPUT07)"

muloe08:
	$(LX) -no-pdf -jobname=$(PROJECT)08Muloe $(TEXFLAGS) "$(MULOE)$(INPUT08)"
	$(LX) -jobname=$(PROJECT)08Muloe $(TEXFLAGS) "$(MULOE)$(INPUT08)"

muloe09:
	$(LX) -no-pdf -jobname=$(PROJECT)09Muloe $(TEXFLAGS) "$(MULOE)$(INPUT09)"
	$(LX) -jobname=$(PROJECT)09Muloe $(TEXFLAGS) "$(MULOE)$(INPUT09)"

muloe10:
	$(LX) -no-pdf -jobname=$(PROJECT)10Muloe $(TEXFLAGS) "$(MULOE)$(INPUT10)"
	$(LX) -jobname=$(PROJECT)10Muloe $(TEXFLAGS) "$(MULOE)$(INPUT10)"


all:	uebung02 uebung04 uebung05 uebung06 uebung07 uebung08 uebung09 uebung10 muloe02 muloe04 muloe05 muloe06 muloe07 muloe08 muloe09 muloe10 


clean:
	cd ./output; rm -f *.adx *.and *.aux *.bbl *.blg *.idx *.ilg *.ldx *.lnd *.log *.out *.rdx *.run.xml *.sdx *.snd *.toc *.wdx *.xdv *.nav *.snm *.bcf *.vrb

