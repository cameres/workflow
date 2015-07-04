# Connor's Workflow for Git/Github Projects
- Using robbyrussel's git plugin
1. Open new branch
  - `$ gb <new-branch>`
2. Move to new branch
  - `$ gco <new-branch>`
3. Connect new branch to origin
  - `$ ggsup <remote> <branch>`
4. Commit/Work on code
  - create(if necessary)/run tests
  - code
  - run tests
  - `$ gcmsg ... `
5. Push code from branch
  - `$ gp ... `
  - *see step 3 if feature is not complete*
6. Create pull request
  - `$ hub pull-request ...`
  - or via browser
7. Merge pull request
  - `$ hub browse`
  - via browser
8. Create a signed tag in master branch
  - `$ gts -m <note> <release>`
  - `$ gp --tags`
9. Either of the following:
  - Delete local branch + origin branch
    - Delete remote branch : `$ gp <remote> :<branch>`
    - Merge branch and delete : `$ gbda <branch>`
  - Keep branch alive
    - branch should stay up to date with master
