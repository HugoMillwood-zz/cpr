# cpr
create pull request - a simple bash script for setting the upstream to origin and opening a GitHub pull request

# Use
If you're tired of trying to copy-paste the `--set-upstream` line over and over again
```
hugo@omar:~/code/androidshell$ git push
fatal: The current branch fix/dumpCore has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin fix/dumpCore

```

you can now just run `cpr`

```
hugo@omar:~/code/androidshell$ cpr
Total 0 (delta 0), reused 0 (delta 0)
remote:
remote: Create a pull request for 'fix/dumpCore' on GitHub by visiting:
remote:      https://github.com/BonnierNews/androidshell/pull/new/fix/dumpCore
remote:
To github.com:BonnierNews/androidshell.git
 * [new branch]          fix/dumpCore -> fix/dumpCore
Branch 'fix/dumpCore' set up to track remote branch 'fix/dumpCore' from 'origin'.
```

Tada :tada:

# Note
This little script does not take into consideration if you're using something other than GitHub or if `xdg-open` is installed or if you've cloned the repository over anything other than ssh. It's just a quick and dirty way to set the upstream and open a GitHub pull request for the current branch. Feel free to modify it however you see fit.
