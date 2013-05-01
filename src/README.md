This repository is for executing a sphinx-build for OSEHRA documentation.  It is independent of current documentation efforts, as this code will be run on a web server to render existing documentation in a more human friendly format.

To execute the build, after installing Sphinx, from the root directory execute the following:

sphinx-build -a -b html -c ./src/sphinx ./src/documentation ./documentation

-a : Always rebuild all files (good for testing themes).
-b : Build format (html for web).
-c : location of sphinx configuration files.

Other operators are source and target directories.

Hopefully, this site may be modified to leverage git hooks to automate build of sphinx documentation.  For now, this is unfortunately a manual process.