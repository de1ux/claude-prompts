## Snapshots

"Run snapshots" usually means `bzl run //:snapshot -- //path/to/thing/...`, but use git diff to figure out if there's staged changes in `//path/to/thing`. Thats a key clue on where to run the snapshots

"Make a PR with ticket number RADI-1234" means to stash the current changes, use `ginit --force RADI-1234`, create a new commit with `gcommit` and run `gsubmit` to create a draft PR.

## Cleanup my Jira tickets

Look for JIRA tickets assigned to me that are 'In progress', or 'In PR' that already have merged Github PRs associated with them. Move these to 'Done'.

## Fix tests

Use git diff to find what files have changed, or if there are no working changes, look at the previous commits. If a file /pkg/lib.go is changed, tests can be run with bzl test //pkg/... to run all tests in that folder. Always use bzl to run tests, very important to never EVER use `go test` directly!

## Missing `go_test` / `go_build` bazel macros

Run `bzl run //:gazelle` to generate these.