# Goal

The purpose of these exercises is for the interviewer to get a sense of how you write code and english. This shouldn’t take you more than a few hours to get done. If you already have code on Github or Bitbucket, or a blog that you feel is representative of your current abilities, you can send us a link to those instead of doing these exercises. Note that you cannot point to work that was done by a group of people - you need to have done all the work yourself.

## Writing exercise

The point of this exercise is to benchmark your writing skills.

Write an approximately 500 word article about something you're passionate about that’s technology related. It doesn't really matter what the topic is. For instance, you can write about a [language feature](https://www.mikeash.com/pyblog/friday-qa-2015-06-19-the-best-of-whats-new-in-swift.html) you like or dislike, something in the [news](http://david-smith.org/blog/2014/11/18/initial-impressions-for-watchkit/), [something](http://daringfireball.net/2014/11/native_apps_are_part_of_the_web) that you have an opinion about, etc.

## Code exercise

The point of this exercise is to benchmark your ability to write code. Although this is a toy problem, please make sure your solution is of production quality. You should be comfortable checking your solution into your primary code base. Use proper names, check for errors, etc. Your code should be representative of how you code on the job.

### Constraints

- You must submit an Xcode 10 project (or higher), targeting iOS 11 or later.
- Your code must be written in Swift 4 or later.
- You may use any libraries of your choice.
- You must provide instructions on how to build and run your code.
- The app must work in both portrait and landscape orientations.

### Submission

The expected submission method is by filing a PR in this repository. Please write back to us with a link to your PR when your work is ready to be looked at.

### Problem

A JSON over HTTP API is deployed at `http://surya-interview.appspot.com`. The goal is to make requests to it and render the data obtained from it in an iOS application.

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

You are to cache this data locally on the device (that is, if you've gotten the data once, the next time your app is opened, it should use the locally stored data to render the view and then update data from the server in the background) and render each of these items in a row inside a `UITableView`.


# Contact

If there's anything you're uncertain about and need clarification, please feel free to reach out to us.
