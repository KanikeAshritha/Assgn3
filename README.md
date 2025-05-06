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

-ESLint: Checks the code for mistakes and keeps the style consistent.

-Prettier: Automatically formats the code to look clean and uniform.

-Husky: Lets us run scripts (like checks or formatting) before making a commit.

-Lint-staged: Runs those checks only on files which are about to commit, saving time.


SET Up process -->

1)npx mrm lint-staged: Run this command in terminal for necessary installations.
2)Edit json package =
"lint-staged": {
 "*.{ts,tsx}": [
  "prettier --write",
  "eslint --max-warnings 0 ."
  ]
}

This setup automatically checks and fixes the code before every commit and it keeps the code clean and avoids errors being pushed into the project and it also saves time and helps everyone on the team write code the same way.
