# Git Cheat Sheet

## Getting Started

<table style="border: 1px solid">
  <tr>
    <th>Commands</th>
    <th>Function</th>
  </tr>
  <tr>
    <td>git init</td>
    <td>Start a new repo</td>
  </tr>
  <tr>
    <td>git clone &lt;url&gt;</td>
    <td>Clone an existing repo</td>
  </tr>
</table>

## Prepare to Commit

<table style="border: 1px solid">
  <tr>
    <th>Commands</th>
    <th>Function</th>
  </tr>
  <tr>
    <td>git status</td>
    <td>Check what you added</td>
  </tr>
  <tr>
    <td>git add &lt;file&gt;</td>
    <td>Add untracked file or unstaged changes</td>
  </tr>
  <tr>
    <td>git add .</td>
    <td>Add all untracked files and unstaged changes</td>
  </tr>
  <tr>
    <td>git add -p &lt;file&gt;</td>
    <td>Choose which parts of a file to stage</td>
  </tr>
  <tr>
    <td>git add rm --cached &lt;file&gt;</td>
    <td>Tell Git to forget about a file without deleting it</td>
  </tr>
  <tr>
    <td>git reset &lt;file&gt;</td>
    <td>Unstage one file</td>
  </tr>
  <tr>
    <td>git reset</td>
    <td>Unstage everything</td>
  </tr>
</table>

## Make Commits

<table style="border: 1px solid">
  <tr>
    <th>Commands</th>
    <th>Function</th>
  </tr>
  <tr>
    <td>git commit</td>
    <td>Make a commit (and open text editor to write message)</td>
  </tr>
  <tr>
    <td>git commit -m "mgs"</td>
    <td>Make a commit</td>
  </tr>
  <tr>
    <td>git commit -am "mgs"</td>
    <td>Commit all unstaged changes</td>
  </tr>
</table>

## Discard Your Changes

<table style="border: 1px solid">
  <tr>
    <th>Commands</th>
    <th>Function</th>
  </tr>
  <tr>
    <td>git checkout &lt;file&gt;</td>
    <td>Delete unstaged changes to one file</td>
  </tr>
  <tr>
    <td>git reset --hard</td>
    <td>Delete all staged and unstaged changes</td>
  </tr>
  <tr>
    <td>git clean</td>
    <td>Delete untracked HEAD &lt;file&gt;</td>
  </tr>
</table>

## Code Archeology

<table style="border: 1px solid">
  <tr>
    <th>Commands</th>
    <th>Function</th>
  </tr>
  <tr>
    <td>git log</td>
    <td>Look at a branch's history</td>
  </tr>
  <tr>
    <td>git log --decorate</td>
    <td>Add reference names</td>
  </tr>
  <tr>
    <td>git log --author="name"</td>
    <td>Filter commits based on the author's name or email</td>
  </tr>
  <tr>
    <td>git shortlog</td>
    <td>Summarizing the output of git log</td>
  </tr>
  <tr>
    <td>git log --graph</td>
    <td>Add a graphical representation of the commit history </td>
  </tr>
  <tr>
    <td>git show &lt;hash&gt;</td>
    <td>Display detailed info about the commit</td>
  </tr>
</table>

## Add a Remote

```
$ git remote add <name> <url>
```

## Push your changes

<table style="border: 1px solid">
  <tr>
    <th>Commands</th>
    <th>Function</th>
  </tr>
  <tr>
    <td>git push origin main</td>
    <td>Push the main branch to the remote origin</td>
  </tr>
  <tr>
    <td>git push -u origin &lt;name&gt;</td>
    <td>Push a branch that you've never pushed before</td>
  </tr>
  <tr>
    <td>git push</td>
    <td>Push the current branch to its remote "tracking branch"</td>
  </tr>
</table>

## Move Between Branches

<table style="border: 1px solid">
  <tr>
    <th>Commands</th>
    <th>Function</th>
  </tr>
  <tr>
    <td>git checkout -b</td>
    <td>Create a branch</td>
  </tr>
  <tr>
    <td>git checkout &lt;name&gt;</td>
    <td>Switch branches</td>
  </tr>
  <tr>
    <td>git branch</td>
    <td>List branches</td>
  </tr>
  <tr>
    <td>git branch -d &lt;name&gt;</td>
    <td>Delete a branch</td>
  </tr>
</table>

## Combine Diverged Branches

<table style="border: 1px solid">
  <tr>
    <th>Commands</th>
    <th>Function</th>
  </tr>
  <tr>
    <td>git rebase main</td>
    <td>Combine with rebase</td>
  </tr>
  <tr>
    <td>git merge &lt;branch&gt;</td>
    <td>Push a branch that you've never pushed before</td>
  </tr>
</table>

## Git Stash

<table style="border: 1px solid">
  <tr>
    <th>Commands</th>
    <th>Function</th>
  </tr>
  <tr>
    <td>git stash</td>
    <td>Temporarily save changes</td>
  </tr>
  <tr>
    <td>git stash save "message"</td>
    <td>Add a descriptive message</td>
  </tr>
  <tr>
    <td>git stash apply</td>
    <td>Reapply the changes saved in the stash.</td>
  </tr>
  <tr>
    <td>git stash list</td>
    <td>List the saved stashes</td>
  </tr>
  <tr>
    <td>git stash clear</td>
    <td>To clear all stashes</td>
  </tr>
</table>
