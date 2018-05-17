# Contributing

First, thank you for your interest and willingness to contribute to this repository!
When doing so, please first discuss the change you wish to make via issues before making a change.

Please note we have a code of conduct, please follow it in all your interactions with the project.

## Development Process

We strive to follow a Git workflow like [this one](http://nvie.com/posts/a-successful-git-branching-model/).

`master` should always be production-ready.
`develop` is for "on-deck" changes – work that will eventually become the next tagged release.

Feature branches should be created off of the latest in `develop`.
All features **must** be tested - PRs that introduce new work or changes without matching tests will be rejected!

Once a feature is thought to be ready for review, the developer should `git fetch develop && git pull --rebase develop` to update their current branch with any recent updates that may have been made by others to the `develop` branch.
The developer is responsible for ensuring that all merge conflicts are addressed appropriately (but please, reach out if you need help!).
With the feature branch updated, the developer may create a pull request from their feature into `develop`, and await review.

After a PR is approved and ready to be merged, a final `git fetch develop && git pull --rebase develop` should be performed, followed by a `git push -f origin <FEATURE>` if necessary.
If everything still looks good, the feature may be merged into `develop` (please **squash** merges to maintain a clean commit history), and the feature branch deleted.

### Collaboration on a Feature

It may be necessary for multiple people to be working on the same feature simultaneously.
It's been my experience that following the same sort of guidelines as above makes this process fairly easy.
Just treat the main feature branch as `develop`, and have each contributor create their own individual branch off of the feature branch.
Create PRs and merge as above as well - make sure that everyone is `git pull --rebase`ing frequently to make keep their local work updated and conflicts to a minimum.

## Code of Conduct

- https://www.python.org/psf/codeofconduct/
- https://www.contributor-covenant.org/version/1/4/code-of-conduct
- As Bill and Ted would say: "Be excellent to each other."
