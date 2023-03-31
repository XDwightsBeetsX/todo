# SASS

SASS refers to both `.sass` and `.scss`.
Of the two, `.scss` is more popular and uses standard `.css` syntax with some extra features.
`.sass` uses indentation-based syntax.

- [SASS](#sass)
	- [Installing SASS](#installing-sass)
		- [Option 1 - Using Chocolatey](#option-1---using-chocolatey)
		- [Option 2 - Download from GitHub](#option-2---download-from-github)
	- [Using SASS](#using-sass)
		- [With Folders](#with-folders)
		- [Single File](#single-file)

## Installing SASS

### Option 1 - Using Chocolatey
1. Follow the steps [here](https://chocolatey.org/install) to download the Chocolatey package manager.
	
	Make sure it works by opening a shell and typing:
	```shell
	ps> choco --version
	```
2. Download SASS by entering the command into an Admin-shell
	```shell
	> choco install sass
	```

	Make sure SASS works by opening a shell and typing:
	```shell
	> sass --version
	```

### Option 2 - Download from GitHub

1. Download the source code from GitHub [here](https://github.com/sass/dart-sass/releases/tag/1.60.0)

2. Add the executable to PATH
	
	Make sure SASS works by opening a shell and typing:
	```shell
	> sass --version
	```

> For Node, install SASS with the command: `> npm install -g sass`
## Using SASS

### With Folders

```shell
> sass --watch src/sass:src/css
```

### Single File

One-time operation:
```shell
> sass input.scss output.css
```

Compiles whenever a change is detected with `watch`:
```
>  sass --watch src/sass:src/css
```
> Compiles folder of sass files in `src/sass` into `.css` files in `src/css`



> See [this](https://sass-lang.com/guide) guide for more information on installing or using SASS
