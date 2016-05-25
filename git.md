

incoming isn't quite a direct mapping in git because you can (and I often do) have multiple repos you're pulling from, and each repo has multiple branches.

If there were an equivalent of hg's incoming command, it'd probably be this:

git fetch && git log ..origin/master

That is, "go grab all of the stuff from the upstream, and then compare my current branch against the upstream master branch."

Similarly, outgoing would be this:

git fetch && git log origin/master..

In practice, I just type those manually (even though I created an alias for one of them) because it's easy to have lots of local branches tracking and being tracked by lots of remote branches and have no trouble keeping it together.
