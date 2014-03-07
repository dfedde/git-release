git-feature
=========== 
This script is designd to help you with the [git workflow]( https://www.atlassian.com/git/workflows#!workflow-gitflow ) by adding a new subcommand, release. release it's self has two commands stage and finalize. the stage command creates a new branch with the prefix release- (this can be changed at the top of the file). when you are done working finalizing that branch finalize it. finalize merges your current code with devbranch and enviroment pushes it back up to the remote and deleates the local feature branch.

Installation
============
All that needs to hapen to make this code work is for git-release to be in the path.
I sugest installing like this

    git clone https://github.com/dfedde/git-release.git /usr/local/share/
    ln -s /usr/local/share/git-release/bin/git-release /usr/bin/

how to use it
=============
to start a new feature 
    
    git release stage <version number>

to finish the feature 
    
    git release finalize [version number]
