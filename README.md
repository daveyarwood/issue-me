# issue-me

Sometimes you want to work on something, but you can't decide what. Or maybe you're worried about your old projects becoming old and neglected. Random number generator to the rescue!

This script uses the GitHub API to find all the open issues for projects you're watching and chooses one for you randomly.

## Setup

### GitHub Username

Set your GitHub username in your environment as `GITHUB_USER`.

### Authorization

The GitHub API requires you to authorize applications to access your user data. `issue-me` needs to be able to see the list of repos that you're watching, as well as the list of open issues for these repos, in order to find you an issue to work on.

To authorize this:

1. [Generate a token in the GitHub UI](https://github.com/settings/tokens). Make sure it has the `repo` and `user` permission scopes.

2. Copy the token to your clipboard, and set it in your environment as `GITHUB_TOKEN`.

### Install

1. Have [Boot](http://boot-clj.com) installed.

2. Clone this repo, and `cd` into it.

3. `chmod +x issue-me && cp issue-me /usr/local/bin`

## Usage

<img align="center" src="https://raw.githubusercontent.com/daveyarwood/issue-me/master/demo.gif" title="issue-me demo" alt="issue-me demo" />
