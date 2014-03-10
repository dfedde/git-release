git-feature
=========== 
This script is designd to help you with the [git workflow]( https://www.atlassian.com/git/workflows#!workflow-gitflow ) by adding a new subcommand, release.
Release it's self has two commands stage and finalize. 
The stage command creates a new branch with the prefix release- (this can be changed at the top of the file). 
When you are done working on that branch finalize it. 
Finalize merges your current code with the devlopment branch and master, pushes it back up to the remote and deleates the local release branch.

Installation
============
All that needs to happen to make this code work is for git-release to be in the path.
I suggest installing like this

    git clone https://github.com/dfedde/git-release.git /usr/local/share/
    ln -s /usr/local/share/git-release/bin/git-release /usr/bin/

This allows you to get updates just by running git pull`in usr/local/share

How to use it
=============
To start a new release 
    
    git release stage <version number>

To finish the release 
    
    git release finalize [version number]
    
Future updates
==============
- deleate release branch from the remote


Change log
==========

v0.1.0
- now pushes to devlopment and master
- sets the tag on master to the version from the branch name

v0.0.1
- nothing this is the first release
