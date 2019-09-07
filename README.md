# Parboiled2 Example
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fanuccio1%2Fparboiled-example.svg?type=shield)](https://app.fossa.io/projects/git%2Bgithub.com%2Fanuccio1%2Fparboiled-example?ref=badge_shield)

This is the full source code for a blog post on parboiled2.

It contains parboiled2 parsers for a simplified version of [Slack Assisted Search](https://get.slack.help/hc/en-us/articles/202528808-Search-for-messages-and-files).
The BNF for our simplified version is:
```
Input  = Term, [ Filter ];
Filter = SearchInChannel | SearchMessagesFrom | SearchOnDate
SearchInChannel = "in:", Term
SearchMessagesFrom = "from:", Term;
SearchOnDate = "on:", Term;
Term = { AlphaNumeric-Character };
```

## Running the examples
If you have a JVM/JDK installed you can run the tests:
```
./sbt test
```
Or you can open a REPL and play with the examples:
```
./sbt console
```


## License
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fanuccio1%2Fparboiled-example.svg?type=large)](https://app.fossa.io/projects/git%2Bgithub.com%2Fanuccio1%2Fparboiled-example?ref=badge_large)