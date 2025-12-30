#Demo 2

Some text. When we make a new repository, simply pushing it will not reflect changes. 
Will will thus have to go to github and create a new repository, then come back here and enter git remote add origin <repository link>. 

Use git remote -v to check which repositories have been added.

NOW, we type git push origin main to update changes to github. If we want it to push 
somehwere by DEFAULT, do git push -u origin main

Try git config --global http.version HTTP/1.1 if normally pushing it via git push origin main does not work.

# Git branching
So far, all of our changes have been made on the main branch. Ie every commit will be along a linear branch.

# So what happens when we branch off?
When we make a branch off of the main branch, the changes made will ONLY be seen in the feature branch. Basically, each branch
ONLY keeps track of changes made on its OWN branch! This is basically a space to write code in a sandbox/demo area to make sure
that it works correctly before we MERGE it back into the main branch. OR eg. we can make a branch off of the main branch to fix a bug in the code, ensure that it works correctly, before merging it back into the main branch. This way, we can prevent
issues like accidentally messing up and making it even worse without a way to go back. Let's try branching!

COMMANDS:
"git branch" shows us how many branches we currently have
"git checkout -b feature" creates a new branch, "feature" is where the name should go.
The branch that we are currently on is highlighed.
Basically, "git checkout" is used to switch between branches

Now, let's test by making some changes on our branch. 


## Local development

1. We made this change on the local branch. 
# Hello? I said we made some modifications!!!ere

# This is a modification made in main
 git commit main

 #Hello????

 Good morning
 hello

 ererer

 # I HAVE MADE CHANGES HERE!!!!!

 To reset changes, do git log, copy the hash of the version that we want to revert to (this is why git commit messags are important!), then git reset <hash> to revert to that specific version!