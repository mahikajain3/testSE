DOCFILES = $(shell ls *.py | sed 's/.py/.html/')
export PKG = API

docs: $(DOCFILES)

%.html: %.py
	pydoc3 -w ./$<
	git add $@

include ../common.mk
