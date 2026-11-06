# Undo Guide

| Situation | Command | Safe after push? |
| --- | --- | --- |
| I broke a file and did not stage it yet | git restore <file> | yes |
| I staged a file by mistake | git restore --staged <file> | yes |
| I made a typo in the last commit message | git commit --amend | no |
| A bad commit is already shared with the team | git revert <id> | yes |
| I want to squash my local commits into one | git reset --soft <id> | no |
| I want to throw away my local commits completely | git reset --hard <id> | no |
| I need a clean working directory for a minute | git stash | yes |
