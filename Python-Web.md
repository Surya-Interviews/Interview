# Goal

The purpose of these exercises is for the interviewer to get a sense of how you write code and english.

## Writing exercise

The point of this exercise is to benchmark your writing skills.

Write an approximately 500 word article about something you're passionate about that’s technology related. It doesn't really matter what the topic is. For instance, you can write about a [language feature](https://www.mikeash.com/pyblog/friday-qa-2015-06-19-the-best-of-whats-new-in-swift.html) you like or dislike, something in the [news](http://david-smith.org/blog/2014/11/18/initial-impressions-for-watchkit/), [something](http://daringfireball.net/2014/11/native_apps_are_part_of_the_web) that you have an opinion about, etc.


## Code exercise

The point of this exercise is to benchmark your ability to write code. Although this is a toy problem, please make sure your solution is of production quality. You should be comfortable checking your solution into your primary code base. Use proper names, check for errors, etc. Your code should be representative of how you code on the job.


### Constraints

- Your solution must be written in Python. Python 3 is preferred, but Python 2 is fine.
- Ideally, you should use either Django (preferred) or Flask, but if you’re unfamiliar with either, feel free to use a framework that you’re comfortable in.
- You are free to use any database you'd like. Explain your choice in your README.
- You may use any other libraries you find useful.
- You must have a README. It must have instructions on how to build, and run your code. It should also include details about database setup.
- Your solution must work (at least) in the latest version of Chrome.

### Submission

The expected submission method is a Github, Bitbucket, or GitLab repository. Please email me a link. If you'd like to use a private repo and give me read access, that’s perfectly fine. My username on Github and Bitbucket is `gps`. It is `gp5` on GitLab.

If that’s not an option (please explain why), email me a zip file.

### Problem

The goal is to design a very basic expense tracking web application. The idea is that the application tracks expenses that are incurred for various clients. An `Expense` must have at least these properties: `timestampOfExpense`, `amount`, `currency`, `title`, `description`. `Expense`s belong to a `Client`. A `Client` must have at least a `name` property.

The application should list all clients in the database (with the ability to create one), and clicking on a client should list all expenses associated with the selected client.

The UI specification is deliberately vague - feel free to come up with a UI that you feel best works for this use case. Please note that the UI should be something you’d feel comfortable shipping to production.


# Contact

If there's anything you're uncertain about and need clarification, please feel free to reach out to me at gps@surya-soft.com.
