# THE GRAPHICS COMPILER
CC 	= gnuplot
CFLAGS 	= -persist
SOURCES = kar.gpl
DATA 	= $(SOURCES:.gpl=.dat)
FIGURES = $(SOURCES:.gpl=.eps)

all:	$(SOURCES) $(DATA) $(FIGURES)

$(FIGURES):	$(DATA) $(SOURCES)
	mkdir figures
	$(CC) $(CFLAGS) $(SOURCES)

clean:
	rm -rf figures/
