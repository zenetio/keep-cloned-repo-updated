# keep-cloned-repo-updated
### How to keep a forked repo updated with original repo

### Terminology
OREPO: original repo - the repo created or maintained by the owner

FREPO: the forked repo that presumably has updates to its wiki, not yet on the OREPO

1. Fork the repo you want to clone

This will create a repo in your remote git workspace

2. Clone the forked repo to your local space

This will create the same repo in your local workspace
```sh
git clone https://github.com/<YOUR-GIT>/<OREPO>.git
```

3. Update the cloned repo with original repo

This will updte your local repo with respect to original repo.
```sh
cd <FREPO>
git remote add upstream htpps://github.com/<OREPO>.git
git fetch upstream
```
4. Update your remote repo
```sh
git push https://github.com/<YOUR-GIT>/<FREPO>.git

And now your repo is updated.
