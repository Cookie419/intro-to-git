# Working Directory
-Area where all the files, directories and changes are living all the time.

# Staging Area
- Files and directories that we explicitly add to the staging area.

# Git Repository
-Where all our snapshots are stored.

# Adding multiple files of a certain file type
Use a wild card noted as *. type  "git add *.html"  and all files of that type are added.

# Adding all files in directory (including hidden)
Note: git add -A adds all files and folders from the directory that you're in.
This is a good command for adding everything in your project, all at one time.

# Removing files
Never did find a really good way. tried all Git suggestions . Finally had to add,commit, and then manually delete files by hand to remove them. What!!! a chore. Nothing worked.
# Ignoring files
Set up gitignore and type in code console, what you want it to ignore. Possible that won't work either.

# Git Branches

-Listing all branches
presently only the Master and Feature brances made.

-Adding a branch
To add a branch we call for it with "Git branch."   And then type "Git checkout -b and <name of file>."


-Changing branches
Type "Git checkout <name of branch You want>.
You will see git says "Switched to branch and <name if file that we switched to>."

While on feature branch if you add file5.html itwill show up in logs as added, but once you return to master branch
You'll note that file5.html disappears. This is because before merge master has no idea what's going on in feature
and vise-versa. If you move from feature to master file5.html disappears from the explorer box in our vs code IDE.
Yet once you you return to feature file5.html returns to it's original spot, and when you check log you'll see file5.html. Logs while in master will also not show file5.html for the same reason, in master unaware in logs also.

-Merging a branch
Type "git merge <branch_name>" to create the bridge that bridges the gap between master and feature branch.
This will make both branches know what's in the others files. the other way would be to use "git checkout master.
and then type "git merge feature" which is a much better idea. So we did this one.

-Removing a branch
Command to git rid of it is "git branch -d <branch_name>." and this is what you would use.
your response should be "Deleted <branch_name> with ( a sha ID #) to identify the deleted branch.(was 85df4c0)
Like that.