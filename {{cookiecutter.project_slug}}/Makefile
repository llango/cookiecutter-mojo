.PHONY: build

test:
	magic run test 

package:
	magic run mojo package  src/{{cookiecutter.project_slug}}/ -o {{cookiecutter.project_slug}}.mojopkg

upload:
	export PREFIX_API_KEY={$PREFIX_API_KEY} & bash scripts/publish.sh

build:
	rattler-build build -r src -c https://repo.prefix.dev/mojo-force -c https://conda.modular.com/max -c conda-forge --skip-existing=all

doc:
	mkdocs serve