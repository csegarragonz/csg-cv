ROOT_DIR	= $(CURDIR)
CONFIG_DIR	= $(ROOT_DIR)/config
MAIN_FILE	= $(ROOT_DIR)/SegarraCarlos_CV.tex

.PHONY: all clean main.pdf

all: main.pdf

main.pdf:
	@latexmk \
		-r $(CONFIG_DIR)/latexmkrc \
		-pdf \
		-interaction=nonstopmode \
		-quiet \
		$(MAIN_FILE)

clean:
	@latexmk -r $(CONFIG_DIR)/latexmkrc -C
