# Lec-3 08.04.2017

## Dynamic connectivity problem

### QuickUnion

* element name === index of element in array
* value of element point to parent element
* root element is point to itself 
  * if index of element === value of element this element is root
* each root element represent a component

#### Example
```javascript
//  1,2,3,4,5
// [ , , , , ]

uf.connect(3,5)

//  1,2,3,4,5
// [ , ,5, ,5]

uf.connect(3,1)

//  1,2,3,4,5
// [1, ,5, ,1]

uf.connect(4,2)

//  1,2,3,4,5
// [1,2,5,2,1]

uf.connect(5,4)

//  1,2,3,4,5
// [2,2,5,2,1]


```
### QuickUnion with weighted

To optimise finding of root element, create one more array, and store there number of elements in component, during `connect` operation always connect smaller component to bigger

### QuickUnion with weighted and pathCompression

for each operation `isConnected` we can optimise path from elements to their roots, bind each element with its root

# Home work

### You should know how to solve next tasks with Git and GitHub

> **Names of all branches should have prefix `git-pract-`**

  1. create new branch from current branch
  2. create new branch from any other branch
  3. removing local branch
      1. create new branch 
      2. push it to remote repository (git push origin new-branch)
      3. remove this branch locally 
  4. get remote branch and modify it locally *before start create remote branch with task 3*
  5. create 2 pullrequest with different branches 
      * changes in each branch should be unique
      * both branches should be created from master
  6. change 2 files and create commit with just one of this file
  7. branch switching with changes *before start create remote branch with task 3*
      1. create new branch from master
      2. make changes 
          * do not commit changes
          * do not lose changes
      3. download remote branch
      4. switch to remote branch
          * you should **not** see your changes
      5. return to new branch and modify your changes
          * you should see your changes

Tths comands can halp you
  * git status
  * git diff
  * git add
  * git commit
  * git checkout
  * git checkout -b new-branch
  * git stash
  * git branch remove
  * git fetch


### Implement quickUnion with weighted


### URLS
 - [slides](https://docs.google.com/presentation/d/1jho6Lhz9pWsqed6INyOZ0KtPkQu5Oo_Gh6bwRn7-4R4/edit?usp=sharing)