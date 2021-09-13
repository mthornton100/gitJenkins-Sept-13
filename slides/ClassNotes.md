## Class Notes

### Administrative Stuff

* Attendance will be taken every day. If there is some reason that you are not able to be in class, then please let me know ASAP
* The class will be highly interactive which means:
  * There will be regular mini-quizzes posed by the instructor
  * There regular round-robin Q&A sessions
  * And by Q&A, it means that both you ask me questions, but I will also ask you questions
* We will break for lunch from 12-1
  * This is your time and will be respected
* There will be a 15 min break about 10:15-ish in the morning and one about 2:30-ish in the afternoon
* There will be no new material presented after about 4-4:30
  * That time will be for deep dive questions and related issues you might want to bring up

### Class Repo

* All materials I use in class, including these notes, will be in the student repository at
  * https://github.com/ExgnosisClasses/gitJenkins-Sept-13
  * The repo will be available until at least Oct 15
  * You may share the materials other than the slides with anyone
    * Provided you don't charge for them
    * The slides are not my intellectual property so....
    * Everything else is either my IP or commons licensed so it is free to share

### VMs

* Virtual machines have been provided for your use
* I will show you how to log into your machine at the start of class
* The AWS domain we are using is "exgnosisteaching"
* Your ID is your first name (Rod) and password is your name with "-Rocks" postpended
  * eg My password would be "Rod-Rocks"

### Introductions

1. Your skill area - developer, tester, etc
2. Current tasking - what sort of work are you currently doing
3. Experience with Git, Jenkins and DevOps
4. Objectives for the class

---

## Basic Command

* config
* init
* add 
* commit
  * commit -m "message"
  * commit -a  // does and add and commit for modified
  * commit -am "xxx" 
  * commit -a -m "xx"
* status
* log

## Commits best practices

- Atomic commits
- change that does one thing
  - bug fix
  - feature add
  - "Fixes bug 453"  "Corrects typos in docs"

---

## Working with the repo

#### Undoing adds

* Moving files from the repository into your working directory
* Add file moves changes to the staging are 
  * restore --staged file  removes changes from the staging area
  * leaves your working copy intact

### Restoring from repo
* Copies the file from the repo and OVEWRITES your working copy
* git restore filename

### Lab

* Create a repository
* Create and add a file and commit
* Edit the file
* Display in the file
* Git add file
  * git status to confirm
  * git restore --staged file
  * git status 

* Edit the file
* display to see edits
* get restore file
* confirm the edits are gone


### Deleting from the Repo
* git rm file
* git mv to rename or move a new directory

### LAb

* create a branch
  * git branch branch-name
  * git checkout -b branchname
  * git checkout branchname
  * git status shows you the branch you are on
  * git log --oneline --graph --decorate --all
* make a commit on the new branch
* see how the log display changes
* switch back and forth 

---

## Fast Forward

make some changes on the branch
do a commit 
switch back to the master branch
do a merge "git merge testing"
delete your other branch
