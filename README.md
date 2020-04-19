# gitx

A command line tool to wrap git command to enforce a custom git commit message convention based on "AngularJS Git Commit Message Conventions".

## How to use

`gitx commit`

In most cases, that's all you need to type. In fact, `gitx` supports the same set of [options](https://git-scm.com/docs/git-commit) as `git commit`. But be noted that if you give any of the following options, it will not prompt for convention, instead it will pass all the parameters to `git` command:

- -m/--message

- -c/--reuse-message

- -C/--reedit-message

- -F/--file
- -t/--template

That's to say the commit message passed in the command line takes priority over the convention.