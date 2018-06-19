# Feed Reader Testing project - Udacity

## Introductions

This is a project provided by [Udacity](https://www.udacity.com/).
In this project a web-based application that reads RSS feeds was provided.
There was already included [Jasmine](http://jasmine.github.io/), thus my job was to create test suites for the functionalities of the application.

## Why this Project?

Testing is an important part of the development process and many organizations practice a standard of development known as "test-driven development". This is when developers write tests first, before they ever start developing their application. All the tests initially fail and then they start writing application code to make these tests pass.

Whether you work in an organization that uses test-driven development or in an organization that uses tests to make sure future feature development doesn't break existing features, it's an important skill to have!

## Getting Started

### Installation

You can easily install this project by cloning it on github or downloading the .zip version

### How does it work

The project originally worked as a RSS fead reader with an hided menu, which when opened using the hamburger menu icon helps the user to reach feeds created by 4 different sources.

### Tests

I created four test suites:

 *RSS Feeds*

 This suite is all about the RSS feeds definitions, the allFeeds variable in our application.
 There are three tests:

  - A test to make sure that the allFeeds variable has been defined and that it is not empty.
  - A test that loops through each feed in the allFeeds object and ensures it has a URL defined and that the URL is not empty.
  - A test that loops through each feed in the allFeeds object and ensures it has a name defined and that the name is not empty.

 *The menu*

 Contains tests about the menu functionality:
  - A test that ensures the menu element is hidden by default.
  - A test that ensures the menu changes visibility when the menu icon is clicked. This test has two expectations: does the menu display when clicked and does it hide when clicked again.

 *Initial Entries*

 Has only one test:
  - A test that ensures when the loadFeed function is called and completes its work, there is at least a single .entry element within the .feed container.

 *New Feed Selection*

Has a single test
  - A test that ensures when a new feed is loaded by the loadFeed function that the content actually changes.
