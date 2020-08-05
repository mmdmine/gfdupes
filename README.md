# gfdupes

Graphical interface for
[fdupes](https://github.com/adrianlopezroche/fdupes) (find duplicates)
command in linux

Currently the tool and `install.sh` have been tested on Kali >=14.04
only.

## How to execute

1. run `install.sh`
2. run `gfdupes`

## Requirements

* Python (>=2.0)
* pygtk (>=2.0)
* gtk
* fdupes

## TO-DO

The code is hurriedly written, and we did not take care of many things:

* Every file is stored as a dictionary entry in python, with its path.
  Thus 2 files with same names but different paths, this case is not
  dealt with.
* The tree structure of directories is made completely beforehand, i.e.,
  those directories which won't even be opened by the user, have their
  subtrees or children within. This needs to be removed. We need to
  create a subtree for a directory only when the arrow besides it is
  clicked.
* For some reason, if a filename contains spaces within it, the program
  does not work
* As mentioned earlier, the code is hurriedly written. It is not object
  oriented. We did not add seperate classes for Hboxes, Vboxes, etc.
* Need to test this on other distributions.
* The VBox showing the tree structure is very big in size and consumes
  lot of redundant space on the screen. Decrease the size.
* Package for debian (after all of the above are done)

## New TODOs

* Cross platform (Linux, macOS, Windows, ...) with another GUI library
  (maybe [Kivy](https://kivy.org))
* Python 3
* Fix some issues with fdupes (check if same file via inode?, if md5
  hash is the same, maybe check also sha512/"diff")
* Use pylint and coverage
* Use github actions for code linting etc.
* Provide packages (AUR, brew, ...) or releases
