# midterm

### Section 1
**Question 1**: The differences among cloning, fetching, and pulling.
> git clone will clone a repo in the directory that you are working in. It sets up a local branch based on the remote's active branch, and also creates a remote called "origin" for the repo cloned from. For example, when I cloned the repo for this midterm, the remote is set to the "https://github.com/adhanji8/midterm/", I have to changed the remote URL to the repo I created in my github account, so I can push my modification to my repo.  

>git pull will pull down from a remote whatever you ask and instantly merge it into the branch you're in when you make the request. Git pull is used when you want to bring a local branch up-to-date with its remote version.   
>git fetch is similar with git pull, except it doesn't merge automatically. It will pull down the remote branch, create a local copy of a remote branch. Then you can create a branch from it and work on the new branch.

### Section 2
The differences between Trello and Asana
| Asana | Trello |
|--------|-------|
| Real-time changes | Boards  |
| Multiple workspaces  | Lists  |
| Activity feed  | Attach photos, drawings, sketches & mockups  |


### Section 3
**Question 1**: what is the .git folder? Where is the object database in this folder?
> The . git folder contains all the information that is necessary for your project in version control and all the information about commits, remote repository address, etc. All of them are present in this folder. It also contains a log that stores your commit history so that you can roll back to history.
> The object database is stored in the folder called objects in .git folder.  

**Question 2**: git hash-object function works?
> git hash-object uses one way hash function(sha-1 in git) to compute the object ID value from the content of a given file. By default the object type is blob if without being specified (-t option). The created object can be written into object database optionally (-w option).  

**Question 3**: Where does git internally store the file names to our files? how are tree objects related to this?
> Git blob objects don't contain file name of the source file, while the tree objects store those info. The tree objects in git represent directories. The contents of a tree object are references to other blobs and trees, where blobs are corresponded with files and trees are with directories.

