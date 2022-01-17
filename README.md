# Amplience QA Engineer technical test

This is a straight forward automation task, with backend (restful, json based api) and frontend html checking.

It shouldn't take more than 2 hours of your time, and all code should be submitted by a public github or gitlabs repo.  Try and include a few commits to indicate how you built-up the tests.  Instructions on how to run should be included in a README.md file included in the repo.


## Requirements:-

### Part 1
* Using any framework of your choice
* Check the github public users API for the userid '6wl'
  * https://api.github.com/users/{userid}

* Check the following in the JSON response body
    * name = Gregory Loscombe
    * id = 15330
    * location = Manchester
    * public repos = 7
    * public gists = 11
    * followers = 12
    * following = 29

* Also check any HTTP headers and response code you see as sensible.
* Try and make the test as flexible as possible

### Part 2
* Using selenium as a driver in any framework, and the resp from the above api
* Validate the HTML presentation layer is correctly displaying the information returned from the api, for the userid '6wl'
    * https://github.com/{userid}
* This test should be flexible enough to allow re-pointing to any userid, and read the data from the API to determine that the frontend should render

* Check the following appears in the page
    * name = Gregory Loscombe
    * location = Manchester
    * public repos = 7
    * public gists = 11
    * followers = 12
    * following = 29

* This should ideally follow page object best practise.
