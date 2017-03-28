# Lec-1 25.03.2017


## Steps to task solve:

1. Make sure that you understand task
    1. solve it on the paper
2. Test it
    1. Create file in test directory for new functionality
    2. Create first simple test
    3. Make sure that it work and fail (run it)
3. Create file for implementation
    1. Implement it
        * Create file for new functionality
        * Write implementation to make test pass
        * Add file into `index.js`
        * Make sure that test pass
4. Add more test if needed
    1. Repeat action 2 and 3

## Git

When you add something to your project
first of all, create a new branch
```
git checkout -b my-new-branch
```

now you can see that you in the new branch with command
```
git branch
```

make your change in the code,
you can see changes in the file with 
```
git status
```

and review your changes with
```
git diff
```

add it to your next commit with comand `add`
for example supose we change `inde.js` and added new test file `test/newTest.js` lets add it
```
git add inde.js test/newTest.js
```

now let's check that it added
```
git status
```

and commit our changes with message that describe what this commit bring to our project
```
git commit -m "added new functionality and test"
```

it also possible commit without `-m` flag just `git commit` in that case will open your standard git editor and you can write multiline message there

after commit, you can lock at your commit history, and find your last committed changes
```
git log
```

after that let's push our branch with name `my-new-branch` and last commit into github
```
git push origin my-new-branch
```

In github page of our project, we can find branch `my-new-branch` and create pull request

Now we wait for mentor review


## Lecture keywords:

1. Node.js
2. NPM
3. TDD 
4. Mocha.js
5. Should.js


## Home Work:

- Set up your environment (especially windows)
- Add in your project tasks from entry test (try to do it in TDD style)
- Make pull request in github

## URLS:

- [JavaScript Style Guide](https://github.com/airbnb/javascript)
- [Should.js documentation](https://shouldjs.github.io/)
- [TDD](https://ru.wikipedia.org/wiki/%D0%A0%D0%B0%D0%B7%D1%80%D0%B0%D0%B1%D0%BE%D1%82%D0%BA%D0%B0_%D1%87%D0%B5%D1%80%D0%B5%D0%B7_%D1%82%D0%B5%D1%81%D1%82%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D0%B5)
- [MDN JavaScript](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference)
- [JavaScript RU](https://learn.javascript.ru/)
- [Node.js api](https://nodejs.org/dist/latest-v6.x/docs/api/)
- [Node.js course](https://www.youtube.com/watch?v=ILpS4Fq3lmw&list=PLsuEohlthXdkRSxJTkmTstWKHgBHsd3Dx)
- [NPM](https://www.npmjs.com/)
