DLLTOOL = i686-w64-mingw32-dlltool

all: \
	$(patsubst %.def,lib%.a,$(wildcard *.def))

lib%.a: %.def
	$(DLLTOOL) -k --def $< --output-lib $@
