# From git to gerrit code transferring script

```
Prerequisites:
* Add ibm repository as "repo_ibm_origin".
Example: `git remote add -f repo_ibm_origin https://github.com/username/repository.git`

Parameters:
* Target branch - pekao (dafault your current branch)
* Target branch - ibm (default 'master' branch)
* Common commit message (default 'aligning commit')
* Temporary branch name (default 'tmp-branch')

Tagging:
You should make the first tag to mark commit, from where you want commit messages to be counted.
Example: `git tag $(date '+%Y-%m-%d-%H-%M-%S') <commitId>`

Attention: script should be added to gitignore on both branches
```