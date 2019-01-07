# Goal

The purpose of these exercises is for the interviewer to get a sense of how you write code and english. This shouldn’t take you more than a few hours to get done. If you already have code on Github or Bitbucket, or a blog that you feel is representative of your current abilities, you can send me a link to those instead of doing these exercises. Note that you cannot point to work that was done by a group of people - you need to have done all the work yourself.


## Writing exercise

The point of this exercise is to benchmark your writing skills.

Write an approximately 500 word article about something you're passionate about that’s technology related. It doesn't really matter what the topic is. For instance, you can write about a [language feature](https://www.mikeash.com/pyblog/friday-qa-2015-06-19-the-best-of-whats-new-in-swift.html) you like or dislike, something in the [news](http://david-smith.org/blog/2014/11/18/initial-impressions-for-watchkit/), [something](http://daringfireball.net/2014/11/native_apps_are_part_of_the_web) that you have an opinion about, etc.


## Code exercise

The point of this exercise is to benchmark your ability to write code. Although this is a toy problem, please make sure your solution is of production quality. You should be comfortable checking your solution into your primary code base. Use proper names, check for errors, etc. Your code should be representative of how you code on the job.


### Constraints

- Your solution must be written as a ReactJS project.
- You may use any libraries of your choice.
- You must provide instructions on how to build and run your code.
- The app must work in the latest version of Chrome.

### Submission

The expected submission method is a Github.com, Bitbucket.com, or Gitlab.com repository. Please email me a link. If you'd like to use a private repo and give me read access, that’s perfectly fine. My username on Github.com and Bitbucket.com is `gps`. My username on Gitlab.com is `gp5`.

If that’s not an option (please explain why), email me a zip file.

### Problem

A JSON over HTTP API is deployed at `http://surya-interview.appspot.com`. The goal is to make requests to it and render the data obtained from it in a React application.

Your app should start with a view that asks the user to enter an email address. You are then to make an HTTP `POST` request to `http://surya-interview.appspot.com/list`. The post body must be a JSON object that looks like this:

```javascript
{
    "emailId": "<email address you got from user>"
}
```

The response will contain a JSON object that looks like this:

```javascript
{
    "items": [
        {
            "emailId": "john@doe.com",
            "imageUrl": "http//something.com/foo.jpg",
            "firstName": "John",
            "lastName": "Doe"
        },
        {
            "emailId": "jane@doe.com",
            "imageUrl": "http//something.com/bar.jpg",
            "firstName": "Jane",
            "lastName": "Doe"
        }
    ]
}
```

Your task is now to render this data in a list.

# Contact

If there's anything you're uncertain about and need clarification, please feel free to reach out to me at gps@surya-soft.com.
