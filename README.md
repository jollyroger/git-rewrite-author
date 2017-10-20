# Mass rewrite author/committer history of a git repository

So you've got lots of repos with misspelled author names, wrong or outdated
emails and you want to fix this. Or you just want your git repos to have a 100%
correct and up to date information on the authors/committers. 

Existing solutions (like [this][1] and [this][2]) allow to rewrite one author
at once but it's to troublesome for you to check and update every spelling
variant of someone's name for all of your repositories. 

Need to fix same multiple authors on multiple repositories? Here's the tool
right for you! Here's the steps to follow:

0. Fill your author information into the .mailmap file in the top dir of your
   git repo. See `mailmap.example` and git-shortlog(1) for more details.
1. Check you haven't missed anything with `git shortlog -sne`.
2. Run this script from the top dir of your git repository.

Have fun!

  [1]: https://help.github.com/articles/changing-author-info/
  [2]: https://github.com/davidfokkema/git-rewrite-author/
