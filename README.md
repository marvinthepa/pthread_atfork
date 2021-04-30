# README

This demonstrates a bug that I ran into when using spring and stackprof while
running tests.

To reproduce, run

```
bundle exec spring rails test test/models/article_test.rb
```

What should happen: the test process should terminate after the test is
finished.
What happens instead: the process hangs after the test is finished.
