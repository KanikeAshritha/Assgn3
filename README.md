###--GitFlow Assgn---

Git link:-  https://github.com/KanikeAshritha/Assgn3


feature/update-styling --> Added basic CSS styling to minfy.html file
feature/add-content --> Added content to same minfy.html file

<img width="960" alt="content-update" src="https://github.com/user-attachments/assets/a2357248-0f32-4a27-a11a-6b46477de69f" />

Merged the feature/add-content branch.

<img width="960" alt="merge-conflict" src="https://github.com/user-attachments/assets/3534944a-d2bd-4203-90c7-c33f490177af" />

A merge conflict occured while attempting to merge feature/update-styling after merging feature/add-content branch.

Thw conflict occured because both the branches made changes to same part of 'minfy.html'.
To resolve the conflict:
I accepted the pull request,then it redirected to resolve the merge conflict and then manually I edited the conflict and merged the feature/update-styling branch to master.

<img width="960" alt="styling-update" src="https://github.com/user-attachments/assets/3e36be39-4337-44c5-874c-7691fded9caf" />

Merged the feature/update-styling branch finally.




---------------------------------------------------------------------------------
Medium(Assignment-2)

The tools are --->

-ESLint: ESLint looks through the code to spot common problems or things that don’t follow the rules — like unused variables or inconsistent quotes.Checks the code for mistakes and keeps the style consistent.It keeps everyone’s code clean, readable  and free of small mistakes before they turn into big ones.

-Prettier: Prettier fixes how the code looks — it lines things up, adds spaces, and organizes it nicely so it’s easier to read.It removes the need to argue about where to put a comma or how many spaces to use more like everyone's code ends up looking the same.

-Husky: Husky connects to Git and runs certain commands right before code is committed.For example,it can run ESLint or Prettier automatically.It makes sure we're not committing messy or broken code.If there’s a problem, the commit gets stopped until you fix it.

-Lint-staged:Lint-staged makes things faster by only running checks on files that are actually trying to commit, not the whole project.Without it,tools like ESLint would check every file, which takes time. This keeps things quick.


SET Up ESLint, Prettier, Husky, and Lint-staged-->

1)Initialize project with command: npm init -y

2)Install necessary packages: npm install --save-dev eslint prettier husky lint-staged

3)Set Up ESLint: npx eslint --init

4)Set Up Husky:
npx husky install => this cmd creates git hook.
add it in scripts =>
"scripts": {
  "prepare": "husky install"
}

5)npx husky add .husky/pre-commit "npx lint-staged": This cmd sets up a pre-commit Git hook that runs lint-staged.

6)"lint-staged": {
  "*.{js,ts,tsx}": [
    "prettier --write",
    "eslint --fix"
  ]
}
Adding a lint-staged section to tell it what to run on which files.

