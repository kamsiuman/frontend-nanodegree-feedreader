# Feed Reader Testing

## Table of Contents

- [Instructions](#instructions)
- [Change Log](#changelog)

## Instructions

1. git clone repo-> https://github.com/kamsiuman/frontend-nanodegree-feedreader.git

2. broswer the index.html and see the feed results followed by the jasmine result

## Change Log

[2018.12.31]] update based on the review cooment
--remove all TODO comments
--fix the ".entrys inside .feed" dom selector...
--remove done()
--fix the issue "previous test left it, this test is not independent" in one of the test
To fix this, you have to call loadFeed twice in the last test. Store oldUrl after the first one (inside the callback function of the loadFeed call), then in it, you have to call it again, and only run the expectation inside the callback function of that loadFeed.
