# Goal

The purpose of these exercises is for the interviewer to get a sense of how you write code and english. This shouldn’t take you more than a few hours to get done.


## Writing exercise

The point of this exercise is to benchmark your writing skills.

Write an approximately 500 word article about something you're passionate about that’s technology related. It doesn't really matter what the topic is. For instance, you can write about a [language feature](https://www.mikeash.com/pyblog/friday-qa-2015-06-19-the-best-of-whats-new-in-swift.html) you like or dislike, something in the [news](http://david-smith.org/blog/2014/11/18/initial-impressions-for-watchkit/), [something](http://daringfireball.net/2014/11/native_apps_are_part_of_the_web) that you have an opinion about, etc.


## Code exercise

The point of this exercise is to benchmark your ability to write code. Although this is a toy problem, please make sure your solution is of production quality. You should be comfortable checking your solution into your primary code base. Use proper names, check for errors, write unit/integration tests, structure your code for long term maintainability etc. Your code should be representative of how you code on the job.


### Constraints

- You must submit an Xcode 11 project, targeting iOS 13.0 and above.
- Your code must be written in Swift 5 or later.
- You may use any libraries of your choice.
- You must provide instructions on how to build and run your code.
- Your app must work in both portrait and landscape orientations, on all iOS devices (all sizes of iPhones and iPads that support iOS 12, including multi tasking modes on iPads).
- Do not use storyboards (we do not use them when we build apps). 
- We strongly encourage you to use a reactive programming framework (we use RxSwift).
- You are required to use UIKit, and not SwiftUI (you are more than welcome to send us a SwiftUI implementation in addition to your UIKit implementation).


### Submission

The expected submission method is a Github.com, Bitbucket.com, or Gitlab.com repository. Please email me a link. If you'd like to use a private repo and give me read access, that’s perfectly fine. My username on Github.com and Bitbucket.com is `gps`. My username on Gitlab.com is `gp5`.

If that’s not an option (please explain why), email me a zip file.

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

If there's anything you're uncertain about and need clarification, please feel free to reach out to me at gps@surya-soft.com.
