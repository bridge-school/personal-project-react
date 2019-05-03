# Bridge Personal Project

## Due Date
Due by 9am on May 13th

## Requirements

- Create a landing page where a user should be able to input a valid git username and submit it.

- After submitting the username, two lists should be displayed: 
    - The most recent repositories (repos) forked by the username provided
    - their most recent pull requests.

- Each of the forked repos should display the name of that repo as a link. When clicked, this should link to the base repo.

- Each of the pull requests should display the title of the pull request as a link. When clicked, this should link to that pull request.

- Each of the pull requests should have, in addition, a visual indicator for whether it is open, closed or merged. This could be colour coded, or just have the status in words next to it.

## Data Source
Your data source is the Github API! You'll be using the events and pull-request endpoints. Using the Github API display:
- the most recent repositories a given user has forked
- the most recent pull requests a user has created

The events endpoint will return all the most recent events (or actions) a user has completed. Everything from opening a pull request to forking a repo to starring a repo. All the different types of events are clarified by a type property. E.g. ForkEvent and PullRequestEvent which you can use to get the info you need. The pull request endpoint will give you the information you need to find out the status of a given pull request (whether its open, closed or merged)

**EXAMPLES**
Users: https://api.github.com/users
Repos: https://api.github.com/users/pkanal/repos
Pull requests: https://api.github.com/repos/bridge-school/bridgeschool.io/pulls

Go to those URLs in your browser to have a look at the JSON response. Its a good idea to copy these as example responses into a file in case you hit the rate limit of the API and that way you can keep on developing.

To view these responses in a nice format, install a chrome extension that helps you view JSON, e.g. https://chrome.google.com/webstore/detail/json-formatter/bcjindcccaagfpapjjmafapmmgkkhgoa?hl=en

## Technical requirements
React and Redux, of course! You should use create-react-app, a convenient way to bootstrap React apps. You'll also want to install dev-tools browser extensions for React and Redux.

You can refer to the finished version of a similar Github app here to get started: https://github.com/melaniebrgr/github-app-with-redux-after/tree/final-20180927-1304.

## Instructions

1. Fork this repository to your own github
2. Clone the forked version of this repository to your computer 
3. Set up create react app and make an initial commit to the master branch of your repo

**Part One**
Complete the requirements outlined above using only React (no Redux) and push it up to the master branch of your repo

**Part Two**
Create a new branch called `redux-solution` and port your React only solution to use Redux. Only complete part two after you have finished part one.

**Submissions**
Once you have completed your personal project we'll provide a Google form for you to submit the link to your repo.

If you have any questions, please reach out on slack on the #help-me or #dev-cohort-7 channel! Happy hacking!
