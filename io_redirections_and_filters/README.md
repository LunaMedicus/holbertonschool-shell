
# Shell, I/O Redirections, and Filters

This project covers the basics of shell scripting, focusing on standard input/output, redirections, and text filtering commands.

## Task List

| Task | Description | Script/Command |
| :--- | :--- | :--- |
| **[0. Hello World](https://www.google.com/search?q=./0-hello_world)** | Print "Hello, World" followed by a new line. | `echo Hello, World` |
| **[1. Confused Smiley](https://www.google.com/search?q=./1-confused_smiley)** | Display a confused smiley `"(Ôo)'`. | `echo "\"(Ôo)'"` |
| **[2. Hello File](https://www.google.com/search?q=./2-hellofile)** | Display the content of `/etc/passwd`. | `cat /etc/passwd` |
| **[3. Two Files](https://www.google.com/search?q=./3-twofiles)** | Display content of `/etc/passwd` and `/etc/hosts`. | `cat /etc/passwd /etc/hosts` |
| **[4. Last Lines](https://www.google.com/search?q=./4-lastlines)** | Display the last 10 lines of `/etc/passwd`. | `tail /etc/passwd` |
| **[5. First Lines](https://www.google.com/search?q=./5-firstlines)** | Display the first 10 lines of `/etc/passwd`. | `head /etc/passwd` |
| **[6. Third Line](https://www.google.com/search?q=./6-third_line)** | Display the third line of the file `iacta`. | `head -3 iacta \| tail +3` |
| **[7. Complex Filename](https://www.google.com/search?q=./7-file)** | Create a file with a complex name containing special characters. | `echo "Best School" > "\*\\\'\"Best School\"\'\\\*$\?\*\*\*\*\*:)"` |
| **[8. CWD State](https://www.google.com/search?q=./8-cwd_state)** | Write the result of `ls -la` into a file named `ls_cwd_content`. | `ls -la > 'ls_cwd_content'` |
| **[9. Duplicate Line](https://www.google.com/search?q=./9-duplicate_last_line)** | Duplicate the last line of the file `iacta`. | `tail -n 1 iacta >> iacta` |
| **[10. No More JS](https://www.google.com/search?q=./10-no_more_js)** | Delete all `.js` files in the current directory and subdirectories. | `find . -type f -name "*.js" -delete` |
| **[11. Directories](https://www.google.com/search?q=./11-directories)** | Count the number of directories and sub-directories. | `find . -mindepth 1 -type d \| wc -l` |
| **[12. Newest Files](https://www.google.com/search?q=./12-newest_files)** | Display the 10 newest files in the current directory. | `ls -1t \| head` |
| **[13. Unique](https://www.google.com/search?q=./13-unique)** | Print only words that appear exactly once from input. | `sort \| uniq -u` |
| **[14. Find Word](https://www.google.com/search?q=./14-findthatword)** | Find lines containing "root" in `/etc/passwd`. | `grep root /etc/passwd` |
| **[15. Count Word](https://www.google.com/search?q=./15-countthatword)** | Count lines containing "bin" in `/etc/passwd`. | `grep -c bin /etc/passwd` |
| **[16. What's Next](https://www.google.com/search?q=./16-whatsnext)** | Display lines containing "root" and 3 lines after them. | `grep -A 3 root /etc/passwd` |
| **[17. Hide Word](https://www.google.com/search?q=./17-hidethisword)** | Display lines (or files) in `/etc/passwd` not containing "bin". | `grep -L bin /etc/passwd` |
| **[18. Letter Only](https://www.google.com/search?q=./18-letteronly)** | Display lines in sshd\_config starting with a letter. | `grep '^[A-Z \| a-z]' /etc/ssh/sshd_config` |
| **[19. A to Z](https://www.google.com/search?q=./19-AZ)** | Replace characters `A` and `c` with `Z` and `e`. | `tr A Z \| tr c e` |
| **[20. Hiago](https://www.google.com/search?q=./20-hiago)** | Remove all letters `c` and `C` from input. | `tr -d c \| tr -d C` |
| **[21. Reverse](https://www.google.com/search?q=./21-reverse)** | Reverse the input string. | `rev` |
| **[22. Users & Homes](https://www.google.com/search?q=./22-users_and_homes)** | Display users and home directories, sorted by user. | `cat /etc/passwd \| cut -d : -f 1,6 /etc/passwd \| sort` |
| **[23. Empty Casks](https://www.google.com/search?q=./23-empty_casks)** | Find all empty files and directories. | `find . -empty -printf %f'\n'` |
| **[24. GIFs](https://www.google.com/search?q=./24-gifs)** | List all `.gif` files, sorted and formatted. | `find . -type f -name "*.gif" -printf "%f\n" \| LC_ALL=C sort -f \| rev \| cut -b 5- \| rev` |
| **[25. Acrostic](https://www.google.com/search?q=./25-acrostic)** | Decode acrostics using the first letter of each line. | `cut -c 1 \| paste -s -d ' ' \| tr -d ' '` |
| **[26. Biggest Fan](https://www.google.com/search?q=./26-the_biggest_fan)** | Parse logs to find the top 11 most active IPs. | `tail -n +2 \| cut -f 1 \| sort \| uniq -c \| sort -n -r \| head -n 11 \| cut -b 9-` |