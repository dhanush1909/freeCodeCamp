# Using Reply Templates

These are some of the standard reply templates that you may use while reviewing pull requests and triaging issues.

> You can make your own with GitHub's built-in [**Saved replies**](https://github.com/settings/replies/) feature or use the ones below.

### Thank you

```markdown
Thank you for your contribution to the page! 👍
We are happy to accept these changes and look forward to future contributions. 🎉
```

### Thank you and congrats

> For thanking and encouraging first-time contributors.

```markdown
Hi @username. Congrats on your first pull request (PR)! 🎉

Thank you for your contribution to the page! 👍
We are happy to accept these changes and look forward to future contributions. 📝
```

### Build Error

```markdown
Hey @username

We would love to be able to merge your changes but it looks like there is an error with the Travis CI build. ⚠️

Once you resolve these issues, We will be able to review your PR and merge it. 😊

---

> Feel free to reference the [Style guide for writing articles](https://github.com/freeCodeCamp/freeCodeCamp#article-title) for this repo on formatting an article correctly so your Travis CI build passes. ✅
>
> Also, it's good practice on GitHub to write a brief description of your changes when creating a PR. 📝
```

### Syncing Fork

> When PR is not up to date with the `master` branch.

````markdown
Hey @username

We would love to be able to merge your changes but it looks like there is an error with the Travis CI build. ⚠️

```bash
Error: ENOTDIR: not a directory, open 'src/pages/java/data-abstraction/index.md'
```

This particular error was not caused by your file but was an old error caused by merging faulty code to the `master` branch. It has since been resolved.

To pass the build, you will have to sync the latest changes from the `master` branch of the `freeCodeCamp/freeCodeCamp` repo.

Using the command line, you can do this in three easy steps:

```bash
git remote add upstream git://github.com/freeCodeCamp/freeCodeCamp.git

git fetch upstream

git pull upstream master
```

If you're using a GUI, you can simply `Add a new remote...` and use the link `git://github.com/freeCodeCamp/freeCodeCamp.git` from above.

Once you sync your fork and pass the build, We will be able to review your PR and merge it. 😊

---

> Feel free to reference the [Syncing a Fork](https://help.github.com/articles/syncing-a-fork/) article on GitHub for more insight on how to keep your fork up-to-date with the upstream repository. 🔄
>
> Also, it's good practice on GitHub to write a brief description of your changes when creating a PR. 📝
````

### Merge Conflicts

> When PR has merge conflicts that need to be resolved.¹

```markdown
Hey @username

We would love to be able to merge your changes but it looks like you have some merge conflicts. ⚠️

Once you resolve these conflicts, We will be able to review your PR and merge it. 😊

---

> If you're not familiar with the merge conflict process, feel free to look over GitHub's guide on ["Resolving a merge conflict"](https://help.github.com/articles/resolving-a-merge-conflict-on-github/). 🔍️
>
> Also, it's good practice on GitHub to write a brief description of your changes when creating a PR. 📝
```

¹ If a first-time-contributor has a merge conflict, maintainers will resolve the conflict for them.

### Duplicate

> When PR is repetitive or a duplicate.

```markdown
Hey @username

It seems that similar changes have already been accepted earlier for this article you are editing, sorry about that. 😓

If you feel you have more to add, please feel free to open up a new PR.

Thanks again! 😊

---

> If you have any questions, feel free to ask questions on the ['Contributors' category on our forum](https://forum.freecodecamp.org/c/contributors) or [our Discord server](https://discord.gg/pFspAhS).
```

### Closing invalid pull requests

> When PR is invalid.

```markdown
Hey @username

Thank you for opening this pull request.

This is a standard message notifying you that we've reviewed your pull request and have decided not to merge it. We would welcome future pull requests from you.

Thank you and happy coding.
```
