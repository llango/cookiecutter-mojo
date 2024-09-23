# {{cookiecutter.project_name}}

{{cookiecutter.project_short_description}}


## package build

```bash
magic run mojo package  src/{{cookiecutter.project_slug}}/ -o {{cookiecutter.project_slug}}.mojopkg
```
or 

```bash
make package
```

## test

```bash
magic run test 
```

or 

```bash
make test
```

## version

version {{cookiecutter.version}}

