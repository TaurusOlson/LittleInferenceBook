MDS=$(wildcard *.md)
PDFS=$(patsubst %.md,%.pdf,$(MDS))


all: $(MDS)
	pandoc $+ -o LittleInferenceBook.pdf

clean:
	rm -fv $(PDFS)


.PHONY: clean
