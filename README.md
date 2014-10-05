agile-git-workflow
==================

A simple GitHub git workflow for agile teams based on issues and pull requests

#Rules
1. Never work on ``master``
2. Pulling ``master`` should never create a merge commit
3. Tests are run after ``pull`` and before ``commit``
3. Describe _Features_ in _Issues_
4. Work on _Issue Specific Feature Branches_
5. Regularly ``git rebase origin/master`` _Feature Branches_ to updated ``master``
6. _Interactive Rebase_ before _Creating Pull Request_
7. _Peer Review Pull Request_
8. _Delete Feature Branch_ after _Pull Request Approval_

#Workflow Steps

##Getting Started
###Possibly Fork Repo
If you do not have write access to the the target repo, then fork it first and then proceed

###Clone the repo
```git clone CLONE_URL```

###Review Issues
The team or Product Owner will need to decide what it is that we are doing and what are the priorities.

For the purposes of the simple workflow the terms _Feature_, _Story_ and _Issue_ are all conflated together to mean a small unit of work which can be completed by a single team member (or pair). In real world projects these terms may represent larger units of work. For this workflow we recommend that all work be iteratively broken down in to small units which can be accomplished relatively quickly by a single team member or pair, and for this documment we shall use the term _Feature_

The  _Features_ should be expressed in some ordered form in some system. In the simplest case this can be done directly in the _GitHub Issues_ for this repo, although in larger projects a more flexible system should be used. 

However it is acheived each _Feature_ should be a short unique indentifier (typically an integer or other code). This _Feature Id_should be referenced in the _Commit Messages_ and _Feature Branches_

A number of _Features_ may be grouped together into a _Sprint_, but this is optional

###Workflow Notes
Following this start, the _Feature Process_ below should be followed repeatedly until the _Sprint_ is complete

##Feature Process (Repeat for each _Feature_)

###Identify the Feature
In _GitHub Issues_ identify the feature you want to work on 

###Pull master updates
```git pull origin master```
This should __never__ result in a _merge commit_ because no one is ever working in ``master``



