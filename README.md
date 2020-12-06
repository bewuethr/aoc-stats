# Advent of Code statistics

This repository contains scripts to generate extended statistics for private
leaderboards on [Advent of Code](https://adventofcode.com).

To configure the scripts, two extra files are needed in the same directory as
the `rankings` executable:

- `boardids` contains the board names, IDs and years for which to build the
  extended stats. The name is what will be used in titles and headers, the ID
  of a private leaderboard can be found at the end of its URL:

  ```
  https://adventofcode.com/20XX/leaderboard/private/view/{{boardid}}
  ```

  and the years are a comma-separated list.

  The first line of `boardids` will be ignored, and tokens are separated by
  blanks. Example:

  ```
  Name          ID   Years to build
  Someboard     123  2015,2016,2017,2018
  Anotherboard  456  2018
  ```

- `cookie` contains the adventofcode.com session cookie as found in, e.g., the
  Chrome Dev Tools under Application > Cookies.
