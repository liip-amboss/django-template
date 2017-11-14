October/November 2017
---------------------
* Support translations out of the box including initial generation of .po files.
  Cookiecutters asks which languages should be supported and which one is the default language
* Added `make translations` to run `makemessages` with the right excludes
* Added script `scripts/import_translations.sh` to import po files from e.g. poeditor.com
* Added `make requirements` to generate the *.txt requirements files
* Added tons of files to .gitignore (pycharm, coverage, *.mo etc.)
* Setup `pytest` testing inside vagrant and GitLab CI (just run `pytest` inside `vagrant ssh` after installing
  test requirements)
* Setup automatic testing on GitLab CI
* Enhanced check migrations script: check if a merge migration is missing (runs automatically on GitLab CI)
* Added CI script `check_fuzzy_translations.sh` which checks if there are any fuzzy translations in .po files
* Logging: Use advanced config with separate log file for info level
