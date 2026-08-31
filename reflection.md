## Creating and managing branches

I kept `main` as the standard branch and did all of my work on separate feature
branches. Before starting anything new, I ran `git checkout main` and I then
created a branch with `git checkout -b feature/`, using a descriptive name for 
easy recognition.

I committed in small, key steps rather than leaving till the end. Each commit 
message described a single change for tracing purposes, and it meant I could 
delete/restore one piece of work without losing the rest.

## Handling the merge conflict

A conflict appeared when two branches edited the same file. Git marked the
overlapping section with `<<<<<<<`, `=======`, and `>>>>>>>`, showing both versions. 
I read both carefully to understand what each was trying to do. If they are 
complementary, I combined them by hand, removed the marker lines, and saved the file. 
I then preview the page to confirm before staging and completing the merge. This is an
important chcek point.

## How pull requests supported quality and collaboration

Opening a pull request is a step between writing code and merging it. Reviewing 
my own diff before requesting a review helped me catch it before submitting.
Reviewer comments raised different questions and because the comment can be 
attached to specific lines, feedback was concrete and easy to act on. The pull 
request is also a documented record of why each change was made, for later reference.