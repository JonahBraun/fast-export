# fast-export, migration tool for hg->git

This is a fork from http://repo.or.cz/w/fast-export.git

I've added one fix so that it doesn't choke on empty branch names.

## Todo:

* Elegantly handle unnamed heads so that -f is not necessary.
* Look into "Not a directory" errors:

error: unable to resolve reference refs/tags/hotfix/2011-06-24: Not a directory
error: Unable to lock refs/tags/hotfix/2011-06-24
error: there are still refs under 'refs/tags/release'
error: Unable to lock refs/tags/release
error: unable to resolve reference refs/tags/hotfix/2011-07-08: Not a directory
error: Unable to lock refs/tags/hotfix/2011-07-08

error: unable to resolve reference refs/tags/hotfix/NNNN-NN-NN: Not a directory
error: Unable to lock refs/tags/hotfix/NNNN-NN-NN
error: there are still refs under 'refs/tags/release'
error: Unable to lock refs/tags/release
error: unable to resolve reference refs/tags/hotfix/NNNN-NN-NN: Not a directory
error: Unable to lock refs/tags/hotfix/NNNN-NN-NN
