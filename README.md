# Advent of Code statistics

This repository contains scripts to generate extended statistics for a private
leaderboard on [Advent of Code](https://adventofcode.com).

To configure the scripts, two extra files are needed in the same directory as
the `rankings` executable:

* `boardid` contains the ID from the private leaderboard. It can be found at
  the end of the URL of the private leaderboard:

  ```
  https://adventofcode.com/201X/leaderboard/private/view/{{boardid}}
  ```

* `cookie` contains the adventofcode.com session cookie as found in, e.g., the
  Chrome Dev Tools under Application > Cookies.
