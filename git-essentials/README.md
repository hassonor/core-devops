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