# Repository Aggregates
## github [aggregates](https://github.com/serrasqueiro/aggregates/)
Refer to `README.md` (a markdown file) for the general repository purpose.

## Modules that are not owned
Git repos that are not owned by me are as follow:
```
git submodule deinit -f gdata-python-client
git submodule deinit -f gdata-python3
git submodule deinit -f openconfig_public
```

## Particular Modules Update
1. *openconfig* -- `git submodule update --recursive --init openconfig_public`
1. Update all to master: `git submodule foreach --recursive "(git checkout master ; echo ...)"`
1. Add official remote: `git remote add upstream git@github.com:openconfig/public.git`
1. Fetch everything: `git fetch --all`
1. Pull from official repo: `git pull upstream master`
1. Push all to our _fork repo_: `git push --all`
