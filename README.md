# FileStruc Notation

FileStruc is a simple, easy-to-read, easy-to-write notation for describing file structures in plain text. It was designed with the intention of providing a straightforward way to explain project structures to both humans and Large Language Models (LLMs) like GPT-4. 

## Syntax

The syntax of FileStruc is designed for simplicity. It uses a single dash (`-`) to represent each level of hierarchy within a directory structure and a forward slash (`/`) to indicate directories. Inline comments are supported with a hash symbol (`#`). 

Here is a basic example:

```filestruc
my_project/
-src/ # source files
--main.py # the main Python file
--utils.py # utility functions
-tests/
--test_main.py # tests for main.py
--test_utils.py # tests for utils.py
-.gitignore # files git will ignore 
-README.md # 
-requirements.txt # project dependencies
```

In this example, `my_project/` is the root directory. `src/` and `tests/` are subdirectories, and `main.py`, `utils.py`, `test_main.py`, `test_utils.py`, `.gitignore`, `README.md`, and `requirements.txt` are files.

Comments are not required, though can be helpful. 

## Rules

1. Every item (file or directory) is preceded by a series of dash (`-`) characters. The number of dashes represents the level of the item in the hierarchy. The root directory is at level 0 and has no dashes before it.
2. Directories are denoted with a forward slash (`/`) after their name. 
3. Comments can be added after a file or directory name by appending a `#` and a space followed by the comment text.

## Contribution

Contributions to the FileStruc project are welcome. Please feel free to submit issues and pull requests.
