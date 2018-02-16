# Goal

The purpose of these exercises is for the interviewer to get a sense of how you write code and english. This shouldn’t take you more than a few hours to get done. If you already have code on Github or Bitbucket, or a blog that you feel is representative of your current abilities, you can send me a link to those instead of doing these exercises. Note that you cannot point to work that was done by a group of people - you need to have done all the work yourself.


## Writing exercise

The point of this exercise is to benchmark your writing skills.

Write an approximately 500 word article about something you're passionate about that’s technology related. It doesn't really matter what the topic is. For instance, you can write about a [language feature](https://www.mikeash.com/pyblog/friday-qa-2015-06-19-the-best-of-whats-new-in-swift.html) you like or dislike, something in the [news](http://david-smith.org/blog/2014/11/18/initial-impressions-for-watchkit/), [something](http://daringfireball.net/2014/11/native_apps_are_part_of_the_web) that you have an opinion about, etc.


## Code exercise

The point of this exercise is to benchmark your ability to write code. Although this is a toy problem, please make sure your solution is of production quality. You should be comfortable checking your solution into your primary code base. Use proper names, check for errors, etc. Your code should be representative of how you code on the job.


### Constraints

- Your solution must be written as a Django project, in either python 2 or python 3.
- You may use any other libraries of your choice.
- You must provide instructions on how to build and run your code.
- The app must work in the latest version of Chrome.

### Submission

The expected submission method is a Github or Bitbucket repository. Please email me a link. If you'd like to use a private repo and give me read access, that’s perfectly fine. My username on Github and Bitbucket is `gps`.

If that’s not an option (please explain why), email me a zip file.

### Problem

The goal is to design a very basic expense tracking Django application. The idea is that the application track expenses that are incurred for various clients. An `Expense` must have at least these properties: `timestampOfExpense`, `amount`, `currency`, `title`, `description`. `Expense` objects belong to a `Client`. A `Client` must have at least a `name` property.

The application should list all clients in the database (with the ability to create one), and clicking on a client should list all expenses associated with the selected client.

The UI specification is deliberately vague - feel free to come up with a UI that you feel best works for this use case. Please note that the UI should be something you’d feel comfortable shipping to production.


# Contact

If there's anything you're uncertain about and need clarification, please feel free to reach out to me at gps@surya-soft.com.
