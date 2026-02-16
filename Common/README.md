# Common Scripts

- `run`: Compiles and then runs a C++ project. This can be one or multiple files. Any arguments after the script's requires ones will be appended to the executable's run command.
  - Example (one file): `run cipher test1.in` executes `g++ -g -Wextra -Wall -o cipher cipher.cpp` then `./cipher test1.in`
  - Example (multiple files): `run rack-o,card,hand deck1.txt` executes `g++ -g -Wextra -Wall -o rack-o rack-o.cpp card.cpp hand.cpp` then `./rack-o deck1.txt`
- `val`: Same as `run` except runs the executable with Valgrind
  - Example: `val cipher test1.in` executes `run cipher test1.in` then `valgrind ./cipher`
