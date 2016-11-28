# Goal

The purpose of these exercises is for the interviewer to get a sense of how you write code and english. This shouldn’t take you more than a few hours to get done.


## Writing exercise

The point of this exercise is to benchmark your writing skills.

Write an approximately 500 word article about something you're passionate about that's technology related. It doesn't really matter what the topic is. For instance, you can write about a [language feature](https://docs.python.org/3/library/asyncio-task.html) you like or dislike, something in the [news](https://www.macstories.net/ios/whatsapp-adds-siri-and-callkit-integration-for-ios-10/), [something](http://daringfireball.net/2014/11/native_apps_are_part_of_the_web) that you have an opinion about, etc.


## Code exercise

The point of this exercise is to benchmark your ability to write code. Although this is a toy problem, please make sure your solution is of production quality. You should be comfortable checking your solution into your primary code base. Use proper names, check for errors, etc. Your code should be representative of how you code on the job.


### Constraints

- Your solution must be written in Python.
- You may use any libraries and tools of your choice.
- You must provide instructions on how to run your code. Please be very specific. If you need libraries to be installed, specify exactly how to do so. Specify how to run your program exactly.


### Submission

The expected submission method is a Github or Bitbucket repository. Please email me a link. If you'd like to use a private repo and give me read access, that's perfectly fine. My username on Github and Bitbucket is `gps`.

If that's not an option (please explain why), email me a zip file.


### Problem

Apple's [developer website](https://developer.apple.com/videos/) has videos from each WWDC from 2012 to 2016 hosted on it. Your goal is to scrape that website, and generate a list of these links to these resources for every video, for each of the sessions:

- HD and SD videos (if available)
- PDFs of slides (if available)

For example, the [2016 Platform state of the union](https://developer.apple.com/videos/play/wwdc2016/102/), should produce a JSON object that looks like this:

```json
{
    "title": "Platforms State of the Union",
    "year": 2016,
    "sessionNumber": 102,
    "hdVideo": "http://devstreaming.apple.com/videos/wwdc/2016/102w0bsn0ge83qfv7za/102/102_hd_platforms_state_of_the_union.mp4?dl=1",
    "sdVideo": "http://devstreaming.apple.com/videos/wwdc/2016/102w0bsn0ge83qfv7za/102/102_sd_platforms_state_of_the_union.mp4?dl=1",
    "presentationSlides": "http://devstreaming.apple.com/videos/wwdc/2016/102w0bsn0ge83qfv7za/102/102_platforms_state_of_the_union.pdf"
}
```

If any of the above fields cannot be scraped, the value must be `null`.

Your program should be executable on the command line, and must output a JSON object.

The JSON object should look like this (please pay close attention to the structure):

```json
{
    "sessions": [
        {
            "title": "Platforms State of the Union",
            "year": 2016,
            "sessionNumber": 102,
            "hdVideo": "http://devstreaming.apple.com/videos/wwdc/2016/102w0bsn0ge83qfv7za/102/102_hd_platforms_state_of_the_union.mp4?dl=1",
            "sdVideo": "http://devstreaming.apple.com/videos/wwdc/2016/102w0bsn0ge83qfv7za/102/102_sd_platforms_state_of_the_union.mp4?dl=1",
            "presentationSlides": "http://devstreaming.apple.com/videos/wwdc/2016/102w0bsn0ge83qfv7za/102/102_platforms_state_of_the_union.pdf"
        },
        {
            "title": "Maximizing Battery Life on OS X",
            "year": 2013,
            "sessionNumber": 701,
            "hdVideo": "http://devstreaming.apple.com/videos/wwdc/2013/701xbx2xqblo39z6tpbdrcz/701/701-HD.mov?dl=1",
            "sdVideo": "http://devstreaming.apple.com/videos/wwdc/2013/701xbx2xqblo39z6tpbdrcz/701/701-SD.mov?dl=1",
            "presentationSlides": "http://devstreaming.apple.com/videos/wwdc/2013/701xbx2xqblo39z6tpbdrcz/701/701.pdf"
        }
    ]
}
```

The JSON object can either be printed to stdout (if so, there must be no other output to stdout), or can be written to a file (if so, your program must accept a path as a command line arg, and write the JSON object to that file).


# Contact

If there's anything you're uncertain about and need clarification, please feel free to reach out to me at gps@surya-soft.com.
