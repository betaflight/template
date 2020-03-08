## Important considerations when opening a pull request:

1. Pull requests will only be accepted if they are opened against the `master` branch. Pull requests opened against other branches without prior consent from the maintainers will be closed;

2. Please follow the coding style guidelines: https://github.com/cleanflight/cleanflight/blob/master/docs/development/CodingStyle.md

3. Keep your pull requests as small and concise as possible. One pull request should only ever add / update one feature. If the change that you are proposing has a wider scope, consider splitting it over multiple pull requests. In particular, pull requests that combine changes to features and one or more new targets are not acceptable.

4. Ideally, a pull request should contain only one commit, with a descriptive message. If your changes use more than one commit, rebase / squash them into one commit before submitting a pull request. If you need to amend your pull request, make sure that the additional commit has a descriptive message, or - even better - use `git commit --amend` to amend your original commit.

5. All pull requests are reviewed. Be ready to receive constructive criticism, and to learn and improve your coding style. Also, be ready to clarify anything that isn't already sufficiently explained in the code and text of the pull request, and to defend your ideas.

6. We use continuous integration (CI) with [Travis](https://travis-ci.com/betaflight) to build build all targets and run the test suite for every pull request. Pull requests that fail any of the builds or fail tests will most likely not be reviewed before they are fixed to build successfully and pass the tests. In order to get a quick idea if there are things that need fixing **before** opening a pull request or pushing an update into an existing pull request, run `make pre-push` to run a representative subset of the CI build. _Note: This is not an exhaustive test(which will take hours to run on any desktop type system), so even if this passes the CI build might still fail._

7. If your pull request is a fix for one or more issues that are open in GitHub, add a comment to your pull request, and add the issue numbers of the issues that are fixed in the form `Fixes #<issue number>`. This will cause the issues to be closed when the pull request is merged;

8. Remove this Text :).
