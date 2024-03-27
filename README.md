# Git usage

## Semantic git commits

See how a minor change to your commit message style can make you a better programmer.

Format: `<type>(<scope>): <subject>`

`<scope>` is optional

### Example

```
feat: add hat wobble
^--^  ^------------^
|     |
|     +-> Summary in present tense.
|
+-------> Type: chore, docs, feat, fix, refactor, style, or test.
```

More Examples:

- :sparkles: `feat`: (new feature for the user, not a new feature for build script)
- :bug: `fix`: (bug fix for the user, not a fix to a build script)
- :memo: `docs`: (changes to the documentation)
- :art: `style`: (formatting, missing semi colons, etc; no production code change)
- :recycle: `refactor`: (refactoring production code, eg. renaming a variable)
- :white_check_mark: `test`: (adding missing tests, refactoring tests; no production code change)
- :wrench: `chore`: (updating grunt tasks etc; no production code change)

### General commit rules

- Limit the commit message to 50 characters
- Capitalize the commit
- Do not end the commit with a period
- Use the imperative mood in the subject line
  - If applied, this commit will ...
- (Use emojis https://gitmoji.dev)
  - :construction: for WIP commits
  - :tada: for the initial commit
  - :arrow_up: for version bumps

## Branch naming

- master
- develop
- hotfix/*
- release/*
- (feature|test|fix|chore|docs|refactor)/*

_chore_: tool changes, configuration changes, and changes to things that do not effect an external user.

Regex: `(feature|test|fix|chore|docs|refactor)(/)([a-z]|-)+`

![git-model](https://nvie.com/img/git-model@2x.png)
