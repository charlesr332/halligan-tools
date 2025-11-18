# Scripts

## Setup
1. Upload all the files in **Scripts** to `~/bin`
1. Connect to your Halligan terminal
1. `cd ~`
1. `echo "use -q comp11" >> .cshrc`
1. `echo "chmod +x ~/bin/*" >> .cshrc`
1. Done! You can now use the scripts by typing their name (ex: `dif test`)

## Descriptions
- `dif`: Executes `diff` against a `.gt` and `.out` file using the inputted name
  - Example: `dif test` executes `diff test.out test.gt`
- `run`: Compiles and then runs a C++ project. This can be one or multiple files. Any arguments after the script's requires ones will be appended to the executable's run command.
  - Example (one file): `run cipher test1.in` executes `g++ -g -Wextra -Wall -o cipher cipher.cpp` then `./cipher test1.in`
  - Example (multiple files): `run rack-o,card,hand deck1.txt` executes `g++ -g -Wextra -Wall -o rack-o rack-o.cpp card.cpp hand.cpp` then `./rack-o deck1.txt`
- `rundiff`: Combines `run` and `dif` into one command. Additional arguments can be pasesd just like `run`.
  - Example: `rundiff cipher test1` executes `run cipher test1.in > test1.out` then `dif test1`
- `val`: Same as `run` except runs the executable with Valgrind
  - Example: `val cipher test1.in` executes `run cipher test1.in` then `valgrind ./cipher`
- `racko`: This is a script specific to CS11 HW10 (Rack-O). It executes all of the `run` and `dif` commands for all included tests.
  - Usage: Execute `racko` in the same directory as your HW10 files
