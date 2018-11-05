# keep-cloned-repo-updated
### How to keep a forked repo updated with original repo

1. Fork the repo you want to clone

This will create a repo in your remote git workspace

2. Clone the forked repo to your local space

This will create the same repo in your local workspace
```sh
git clone https://github.com/<YOUR-GIT>/<REPO-YOU-WANT-TO-CLONE>.git
```

3. Update the cloned repo with original repo

This will updte your local repo with respect to original repo.
```sh
cd <TO-CLONED-REPO>
git remote add upstream htpps://github.com/<ORIGINAL-REPO-YOU-CLONED>.git
git fetch upstream
```
4. Update your remote repo
```sh
git push https://github.com/<YOUR-GIT>/<REPO-YOU-WANT-TO-UPDATE>.git

And now your repo is updated.
