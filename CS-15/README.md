# CS-15 Scripts

- `ms`: Makes your MetroSim then runs reference and yours to compare outputs with given station and commands files
  - Example: `ms 1 1` uses station file `test/s1` and commands file `test/c1` to output to `test/s1c1/s1c1.out.me` then compares to `test/s1c1/s1c1.out.ref` (among other comparisons)
- `msval`: `ms` but with Valgrind
- `tw`: For Typewriter, see header comment inside for documentation
- `twval`: `tw` but with Valgrind
- `twall`: Runs `tw` and `twval` for 3 key and 3 text files
