# 05- Comparing Branches

## Log differences

We can compare branches to see different commits between them. To do so use the command `git log <first-branch>..<second-branch>`. This will return all the commits that are in `<second-branch>`, and not in `<first-branch>`.

```zsh
❯ git log main..bugfix-lesson
commit 6572ee7da7ce8b30c0c42cf2d6f27f6968c6b470 (HEAD -> bugfix-lesson)
Author: Miguel Pimenta <jmiguelpimenta@gmail.com>
Date:   Wed Mar 10 20:18:39 2021 -0300

    add details to lesson
```

It is also possible to use the `--oneline` option, `git log --oneline main..bugfix-lesson`.

## See differences

To compare the actual changes between branches we use the `diff` command, like so `git diff main..bugfix-lesson`.