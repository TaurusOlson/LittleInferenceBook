MDS=$(wildcard *.md)
PDFS=$(patsubst %.md,%.pdf,$(MDS))


all: $(MDS)
	pandoc $+ -o LittleInferenceBook.pdf

clean:
	rm -fv $(PDFS)

%.pdf: %.md
	pandoc $+ -o $@

.PHONY: clean
