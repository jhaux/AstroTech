CC = g++
LIBS = 
CFLAGS = -Wall -O3 -std=c++11
NAME = $(notdir $(shell pwd))
BINDIR=./bin
SRCDIR=./src
DOCDIR=./doc
OBJECTS = ${BINDIR}/main.o
GARBAGE = *.{aux,log}


LATEX = pdflatex  # latex compiler
PYTHONTEX = pythontex  # to execute pythoncommands in the tex-file


compile: ${OBJECTS}
		${CC} -o ${BINDIR}/${NAME} ${OBJECTS} ${LIBS}

${BINDIR}/%.o: ${SRCDIR}/%.cpp
			$(CC) -c $(CFLAGS) $< -o $@

all: compile, docu

docu:
		$(LATEX) --shell-escape $(DOCDIR)/$(NAME).tex

.PHONY: clean
clean:
		rm $(GARBAGE)  # remove all auxillary latex files
