Recursive Git Bash Command
==========================
This is a handy script for recursively running git commands in a parent directory.

## Install
Add this script to your PATH. On OSX you'll edit your ```~/.profile``` with:

```
export PATH=/Path/To/recursive-git-bash:$PATH
```

And you'll have ```rgit``` on your path.

## Examples
```
bernies-mbp:git bernieperez$ ll
total 32
drwxr-xr-x  13 bernieperez  staff    442 Jun 17 21:33 ./
drwxr-xr-x+ 60 bernieperez  staff   2040 Jun 17 20:28 ../
drwxr-xr-x  10 bernieperez  staff    340 Jun 17 11:20 express-partial-response/
drwxr-xr-x  23 bernieperez  staff    782 Jun 17 21:31 another-git-project/
drwxr-xr-x   6 bernieperez  staff    204 Jun 17 21:47 recursive-git-bash/

bernies-mbp:git bernieperez$ rgit status
/Users/bernieperez/git/express-partial-response/
# On branch master
nothing to commit, working directory clean
/Users/bernieperez/git/another-git-project/
# On branch master
nothing to commit, working directory clean
/Users/bernieperez/git/recursive-git-bash/
# On branch master
nothing to commit, working directory clean
```

You can run status, pull, branch, the same git command across multiple projects.

## Testing
Works on OSX
