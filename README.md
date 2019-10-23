# Bridge Personal Project

## Due Date
Due by 9am on November 4th 2019

## Wireframes
For reference we have created an invision prototype to show you the flow of the react application which can be found here: https://bridgeschool.invisionapp.com/public/share/5GWTMSJMH

Please note that you do not need to style the application to match this prototype, it is purely to show you the flow of the application. Feel free to style the application as much (or as little) as you'd like.

## Requirements

- Create a search form with an input that allows you enter a GitHub username and button to fetch the user information for the inputted GitHub username

- After clicking the search button, you should make an API call to fetch the inputted username's information

- When user information has been returned, hide the form and display the github username with two lists:
    - The most recent repositories (repos) forked by the username provided
    - their most recent pull requests.

- Each item in the forked repos list should:
    - Display the name of the repo as a link— when this link is clicked it should take you to that repo in a new tab
    - Display the name of the repo it was forked from
    
 - Each item in the pull request list should:
     - Display the name of the pull request as a link— when this link is clicked it should take you to that pull request in a new tab
     - Display the current status of the pull request (Open, Merged, Closed). This can be done by colour coding the list item or display the status in words

- While we recommend trying Test Driven Development (TDD) and writing tests for all of your components, reducers, and helper functions, we ask that you write at least one component test and one helper function test

## Data Source
Your data source is the Github API! You'll be using the user, repos, events, and pull requests endpoints. Using the Github API display:

- The username
- The most recent repositories a given user has forked
- The most recent pull requests a user has created

The events endpoint will return all the most recent events (or actions) a user has completed. Everything from opening a pull request to forking a repo to starring a repo. All the different types of events are clarified by a type property. E.g. ForkEvent and PullRequestEvent which you can use to get the info you need. The pull request endpoint will give you the information you need to find out the status of a given pull request (whether its open, closed or merged)

**EXAMPLES**
- Users: https://api.github.com/users
- Repos: https://api.github.com/users/pkanal/repos
- Events: https://api.github.com/users/pkanal/events
- Pull Request: https://api.github.com/repos/bridge-school/bridgeschool.io/pulls/39

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

If you have any questions, please reach out on slack on the #help-me or #dev-cohort-9 channel! Happy hacking!

## Stretch Goals

### Create tests
Create unit tests for your:
- Reducer(s)
- Components
- Any other helper functions your created

### Error handling
Create a form error for when an invalid username is searched prompting the user to try another name

### Search another user
Add a back button to go back to the form to search for another github user
