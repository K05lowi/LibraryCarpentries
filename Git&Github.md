Hvis jeg har forstået det korrekt, laver jeg en fork på github til min 
egen konto.

Den cloner jeg så til min lokale maskine.

Her arbejder jeg på tingene.

Når jeg er færdig med at skrive i denne fil, adder jeg i min lokale git.
Dernæst comitter jeg.
Og så skriver jeg git push.

Herefter ligger ændringerne i min lokale fork.

Så laver jeg en pull-request på den. 

Hvorefter nogen (Det var vist mig, men burde nok have været Lorna) 
merger mine ændringsforslag ind i stammen af dokumentet.

# Concepts

**Fork** - create a copy of a repos that can be modified.
Forked projects can be seen on your GitHub account.

**Clone** - clone online repos to hardrive as a local copy

**Branch** - different version of a project

**Remote** - an alias pointing to an online repos

**Staging area** - where you modify files locally. You need to 
Git Add files to staging area to modify them

**Fetch** - download current state of online repos without modifying 
your local repos.

**Merge** - merge modification of a branch into current working branch

**Pull** - combination of git fetch and git merge. 
Fetches information from online repos branch and merges to local copy

**Add** - git add specifies which files to add to staging area

**Commit** - snapshot of staging area, making it ready to be pushed to
online repos

**Push** - git push takes all locally commited changes and uploads them to
remote repos branch

## Process
Clone the repository from Github to git
Navigate to the directory in GitBash
Make a working branch (git branch branch_name)
Make the branch the active one you are working on (git checkout branchname)
Target most recent version that is linked to the upstream remote and pull
contents of its development into our active local branch (git pull)

open the file you want to work on, do your thing and save it.

git add to add the modified file(s) to staging area
git commit to take a snap shot of the changes
git push to send the snapshot to the online repos for review 

In GitHub create a **Pull** request. Make sure you are comparing the Master with your branch.
Request review, add and solve comments as necessary and merge the two branches

## Quick review of process

Når jeg forker projektet er det på webben.

Når jeg efterfølgende kloner det til min lokale maskine, sker det i terminalen.

Redigering, add, commit og push sker også på terminalen.

Dernæst er der pull-requestet. Det sker på web.

Og når jeg reviewer og merger, sker det også på webben.

## Additions to LC lesson

Workflow for review and merging (and tidying up) in Github

Find bedre diagrammer til at illustrere processen "push, pull, fork"

Vi svaner også rationalet for hvorfor GitHub er en del af LC ”grundpakken”.




