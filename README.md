# Sources for environment

## Structure

* Each program is stored into a git submodule.
* Each program configuration and modification is stored in the directory of the same name
* If multiple modifications have to be applied there have to be applied in order
* Each programm holds his modifications into a `patches` directory
* **Submodule changes must not be committed** unless the original submodule master branch changes. In this case, only reference to master branch must be committed

## Program modifications

* Programs are modified by applying patches
* Patches are applied in order
* A new branch has to be created from master to apply patches
* A commit has to be performed between each patch application
* If conflicts occurs from a patch
    * Apply patch manually (by retyping the code)
    * Create a custom diff to append to the patch list
    * Commit job

## How to build?

* Go into the program directory folder
* Copy its configuration and apply its patches in order
* Build program

## Improvements

- [ ] Find a solution to manage sources easier than a submodule
- [ ] Create a Makefile or an install script to build prgramm in a simple way

