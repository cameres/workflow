# Connor's Workflow for Git/Github Projects
1. Open new branch
  - `$ git branch <new-branch>`
2. Move to new branch
  - `$ git checkout <new-branch>`
3. Connect new branch to origin
  - `$ git push --set-upstream <remote> <branch>`
4. Commit/Work on code
  - create(if necessary)/run tests
  - code
  - run tests
  - `$ git commit ... `
5. Push code from branch
  - `$ git push ... `
  - *see step 3 if feature is not complete*
6. Create pull request
  - `$ hub pull-request ...`
  - or via browser
7. Merge pull request
  - `$ hub browse`
  - via browser
8. Create tag in master branch
  - `$ git tag <release>`
  - `$ git push --tags`
9. Either of the following:
  - Delete local branch + origin branch
    - Delete remote branch : `$ git push <remote> :<branch>`
    - Delete local branch : `$ git branch -d <branch>`
  - Keep branch alive
    - branch should stay up to date with master
