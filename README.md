# Shell, init files, variables and expansions

This directory contains scripts demonstrating shell initialization, variable handling, and expansions.

## Scripts

* **[0-alias](./0-alias)**: Creates an alias `ls` that executes `rm *`.
* **[1-hello_you](./1-hello_you)**: Prints "hello" followed by the current username (`$USER`).
* **[2-path](./2-path)**: Appends `/action` to the `PATH` environment variable.
* **[3-paths](./3-paths)**: Counts the number of directories in the `PATH`.
* **[4-global_variables](./4-global_variables)**: Lists all environment variables using `printenv`.
* **[5-local_variables](./5-local_variables)**: Lists all local variables, environment variables, and functions using `set`.
* **[6-create_local_variable](./6-create_local_variable)**: Creates a local variable `BEST` with the value "School".
* **[7-create_global_variable](./7-create_global_variable)**: Creates a global (exported) variable `BEST` with the value "School".
* **[8-true_knowledge](./8-true_knowledge)**: Prints the result of adding 128 to the variable `TRUEKNOWLEDGE`.
* **[9-divide_and_rule](./9-divide_and_rule)**: Prints the result of dividing `POWER` by `DIVIDE`.
* **[10-love_exponent_breath](./10-love_exponent_breath)**: Prints the result of `BREATH` raised to the power of `LOVE`.
* **[11-binary_to_decimal](./11-binary_to_decimal)**: Converts a binary number stored in `BINARY` to decimal.
* **[12-combinations](./12-combinations)**: Prints all two-letter combinations (a-z), excluding "oo".
* **[13-print_float](./13-print_float)**: Prints a number with exactly two decimal places.
* **[14-decimal_to_hexadecimal](./14-decimal_to_hexadecimal)**: Converts a decimal number to hexadecimal.
* **[15-rot13](./15-rot13)**: Encodes and decodes text using ROT13 encryption.
* **[16-odd](./16-odd)**: Prints every other line from the input, starting with the first line.
* **[17-water_and_stir](./17-water_and_stir)**: Adds numbers in custom bases (`water` and `stir`) and outputs in base `bestchol`.
