### Git essentials commands
___

#### Staging Changes:
* Saving time in the short term can have consequences
* It's a good idea to discriminately add code

#### Explicit vs. Implicit
* `git push` is quicker
* `git push <remote> <branch>` may prevent problems

#### Undo a commit
1. `git commit -m "some commit"`
2. `git reset --soft HEAD~1`
3. `git status`
4. Results: the commit from step 1 back to `Changes to be committed`

#### Git Hooks
* Allow actions to be tied to stages of development
* May prevent bad code from getting committed
* Easier to implement using various tools
  * Python: pre-commit
    * `pip install pre-commit`
    * `pre-commit install` 
  * Node: husky

#### Git Log
* Great check out  before large commit or merge
* May come in handy when you "git" lost
* `git log` or `git log --oneline` or `git log --graph --oneline`

#### Amend and Revert
* __Amending__
  * Lets you quickly modify a commit 
  * Should be used before pushing
  * E.g.: `git commit --amend -m "feat: some changes"`
* __Reverting__
  * Safely reverts changes of a commit 
  * Does not delete changes
  * E.g.:  `git revert <Some GitCommit Id>` ,  :wq and Enter.