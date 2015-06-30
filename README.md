# Connor's Workflow for Git/Github Projects
1. Open new branch
  - `$ git branch -m <branch>`
2. Connect new branch to origin
  - `$ git push --set-upstream <remote> <branch>`
3. Commit/Work on code
  - create(if necessary)/run tests
  - code
  - run tests
  - `$ git commit ... `
4. Push code from branch
  - `$ git push ... `
  - *see step 3 if feature is not complete*
5. Create pull request
  - `$ hub pull-request ...`
  - or via browser
5. Merge pull request
  - `$ hub browse`
  - via browser
7. Create tag in master branch
  - `$ git tag <release>`
  - `$ git push --tags`
6. Either of the following:
  - Delete local branch + origin branch
    - Delete remote branch : `$ git push <remote> :<branch>`
    - Delete local branch : `$ git branch -d <branch>`
  - Keep branch alive (ex: hot-fix)
    - Must update hot-fix on changes
    - branch should stay up to date with master
