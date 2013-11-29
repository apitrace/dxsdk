DLLTOOL = x86_64-w64-mingw32-dlltool

all: \
	$(patsubst %.def,lib%.a,$(wildcard *.def))

lib%.a: %.def
	$(DLLTOOL) --def $< --output-lib $@
