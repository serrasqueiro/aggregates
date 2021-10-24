# aggregates
Aggregate of other public repositories
+ This is named [aggregates](https://github.com/serrasqueiro/aggregates), at github [serrasqueiro](https://github.com/serrasqueiro/)

## How-To in a nutshell

1. Initialize sub-modules
   + `git pull && git submodule update --init`
   + append with `--recursive` if you are in a hurry,
   + or the module name, e.g. `ggle/libphonenumber`, if you need a particular sub-module.
1. Checkout all modules
   + `git submodule foreach --recursive git checkout master`

## Special notes

* urllib3 fork is just a fork to keep _master_ as the main branch.
