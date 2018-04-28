# friendr
full-stack app that matches users with friends based on survey input, using a Node/Express server.

### Overview

A mock dating app. Takes results from users' surveys, compares their answers with those from other users. The app will then display the name and picture of the user with the best overall match.


### Demo Site

* Check out [this demo version of the site](https://friend-finder-fsf.herokuapp.com/). Use this as a model for how we expect your assignment look and operate.

### Instructions

1. Navigate to the survey page, which includes 10 questions about your personality. Answer every question on a scale of 1 to 5 based on how much you agree or disagree with the statement.

2. Use links on the bottom to see [Github repo](https://github.com/jkhwu/friendr) and current users in JSON format.

3. App will determine your most compatible friend based on how well your answers match:

- - -

### Access

This app can also be accessed from my [portfolio page](https://jkhwu.github.io/Responsive-Portfolio/portfolio.html?vs=1).

- - -

### What I Learned

* logic for finding best matches based on survey responses: getting the sum of the absolute values of the differences between each user's answers to the same questions.
* declaring the PORT variable as `process.env.PORT || 8080` is necessary to deploy to Heroku.
* The Express method `app.use` can sometimes prevent `app.get` requests below from working. Change to `app.get` to avoid this problem.
* how to use the Node package [Path](https://www.npmjs.com/package/path) to join directory paths.
* how to create JSON seed data in a js file.
* using Express method res.JSON(data) to send JSON data while handling a GET or POST request.