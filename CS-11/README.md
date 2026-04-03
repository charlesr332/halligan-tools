# CS-11 Scripts

- `dif`: Executes `diff` against a `.gt` and `.out` file using the inputted name
  - Example: `dif test` executes `diff test.out test.gt`
- `rundiff`: Combines `run` and `dif` into one command. Additional arguments can be pasesd just like `run`.
  - Example: `rundiff cipher test1` executes `run cipher test1.in > test1.out` then `dif test1`
