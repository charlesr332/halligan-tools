# CS-11 Scripts

- `dif`: Executes `diff` against a `.gt` and `.out` file using the inputted name
  - Example: `dif test` executes `diff test.out test.gt`
- `rundiff`: Combines `run` and `dif` into one command. Additional arguments can be pasesd just like `run`.
  - Example: `rundiff cipher test1` executes `run cipher test1.in > test1.out` then `dif test1`
- `racko`: This is a script specific to CS11 HW10 (Rack-O). It executes all of the `run` and `dif` commands for all included tests.
  - Usage: Execute `racko` in the same directory as your HW10 files
- `rackoval`: Similar to `racko` except runs Valgrind for each test, printing the output in console
  - Usage: Execute `rackoval` in the same directory as your HW10 files
- `sushigo`: Similar to `racko` except it's for CS11 HW11 (Final Project: Sushi Go!)
  - Usage: Execute `sushigo` in the same directory as your HW11 files and press any key to advance tests
- `sushigoval`: Similar to `sushigo` except runs Valgrind for each test, printing the output in console
  - Usage: Execute `sushigoval` in the same directory as your HW11 files and press any key to advance tests
