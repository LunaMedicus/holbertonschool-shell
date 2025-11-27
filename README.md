# Shell, init files, variables and expansions
Each file here is a script that execute a basic command from the shell. 
# Shell: Init Files, Variables, and Expansions

* [Task 0](./0-alias) - Create a script that creates an alias. alias  ls="rm *"
* [Task 1](./1-hello_you) - Create a script that prints hello user, where user is the current Linux user. **echo hello $USER**
* [Task 2](./2-path) - Add /action to the PATH. /action should be the last directory the shell looks into when looking for a program. **export PATH=$PATH:/action**
* [Task 3](./3-paths) - Create a script that counts the number of directories in the PATH. **echo $PATH | tr ":" "\n" | wc -l**
* [Task 4](./4-global_variables) - Create a script that lists environment variables. **printenv**
* [Task 5](./5-local_variables) - Create a script that lists all local variables and environment variables, and functions. **set**
* [Task 6](./6-create_local_variable) - Create a script that creates a new local variable. **BEST="School"**
* [Task 7](./7-create_global_variable) - Create a script that creates a new global variable. **export BEST=School**
* [Task 8](./8-true_knowledge) - Write a script that prints the result of the addition of 128 with the value stored in the environment variable TRUEKNOWLEDGE, followed by a new line. **echo $(( TRUEKNOWLEDGE + 128 ))**
* [Task 9](./9-divide_and_rule) - Write a script that prints the result of POWER divided by DIVIDE, followed by a new line. **echo $(($POWER / $DIVIDE))**
* [Task 10](./10-love_exponent_breath) - Write a script that displays the result of BREATH to the power LOVE. **echo $(( BREATH ** LOVE))**
* [Task 11](./11-binary_to_decimal) - Write a script that converts a number from base 2 to base 10. **echo $((2#$BINARY))**
* [Task 12](./12-combinations) - Create a script that prints all possible combinations of two letters, except oo. **echo {a..z}{a..z} | tr ' ' '\n' | grep -v 'oo'**
* [Task 13](./13-print_float) - Write a script that prints a number with two decimal places, followed by a new line. **printf "%0.2f\n" "$NUM"**
* [Task 14](./14-decimal_to_hexadecimal) - Write a script that converts a number from base 10 to base 16. **printf "%x\n" $DECIMAL**
* [Task 15](./15-rot13) - Write a script that encodes and decodes text using the rot13 encryption. Assume ASCII. **tr 'a-zA-Z' 'n-za-mN-ZA-N'**
* [Task 16](./16-odd) - Write a script that prints every other line from the input, starting with the first line. **perl -ne 'print if (++$x)%2'**
* [Task 17](./17-water_and_stir) -  in the environment variables WATER and STIR and prints the result. WATER is in base water, STIR is in base stir, The result should be in base bestchol.
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
