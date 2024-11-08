all: main.pdf

main.pdf:
	docker run --rm \
	  -v $(shell pwd):/workdir \
	  -u $(shell id -u):$(shell id -g) \
	  csegarragonz/latex-docker:texlive_2023 SegarraCarlos_CV.tex

.PHONY: main.pdf

clean:
	docker run --rm \
	  -v $(shell pwd):/workdir \
	  -u $(shell id -u):$(shell id -g) \
	  csegarragonz/latex-docker:texlive_2023 clean
