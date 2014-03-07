git-feature
=========== 
This script is designd to help you with the [git workflow]( https://www.atlassian.com/git/workflows#!workflow-gitflow ) by adding a new subcommand, feature. feature it's self has two commands start and finish. the start command creates a new branch with the prefix branch- (this can be changed at the top of the file). when yu are done working with that feature you can run finish. finish pulls the remote devbranch and merges your current code with devbranch pushes it back up to the remote and deleates the local feature branch.

Installation
============
All that needs to hapen to make this code work is for git-feature to be in the path.
I sugest installing like this

    git clone https://github.com/dfedde/git-feature.git /usr/local/share/
    ln -s /usr/local/share/git-feature/bin/git-feature /usr/bin/

how to use it
=============
to start a new feature 
    
    git feature start

to finish the feature 
    
    git feature finish [feature name]
