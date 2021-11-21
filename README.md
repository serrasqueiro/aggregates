# aggregates
Aggregate of other public repositories
+ This is named [aggregates](https://github.com/serrasqueiro/aggregates), at github [serrasqueiro](https://github.com/serrasqueiro/)

## How-To in a nutshell

1. Initialize sub-modules
   + `git pull && git submodule update --init`
   + append with `--recursive` if you are in a hurry,
   + or the module name, e.g. `ggle/libphonenumber`, if you need a particular sub-module.
1. Checkout all modules
   + to ensure everything is in _master_ branch:
     - `git submodule foreach --recursive git checkout master`
   + or, better, if you are standing with your old checked-out repo, also get updates:
     - `git submodule foreach --recursive "(git checkout master; git pull)"`

## Special notes

### urllib3 fork
* urllib3 fork is just a fork to keep _master_ as the main branch.

### pyang fork
* pyang fork, do:
  + `git submodule foreach '[[ ! $sm_path = pyang ]] || git remote add upstream git@github.com:mbj4668/pyang.git'`
  + and: `git submodule foreach '[[ ! $sm_path = pyang ]] || git checkout new/ietf_no_41'`
