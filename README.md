# PR-METRICS

Project to extract some metrics related with pull requests and development process

## How does it work?

This project uses the Github API to extract information about the merged pull requests given a period of time.

**Command**

`npm start`

**Example**

![Example screencast](docs/example.gif)

**Enviroment variables**

_.env_

<pre>
GITHUB_TOKEN=your-github-token
REPO_OWNER=repo-owner
REPO_NAME=repo-name
</pre>

You need a GitHub token with the right permission in your repository.

**Note:** The application automatically reads _.env_ file in the execution path.

## Pull request metrics

**Time to first review:** time between opening date and first review date

**Time to get needed approves:** time between first review date and needed approves date

**Time to review:** time between first review date and merged date

**Time to merge:** time between opening date and merged date

**Files changes:** number of files changes in the pull request

**Changes:** total changes in the pull request (additions + deletions)
