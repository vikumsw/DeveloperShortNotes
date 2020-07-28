# Developer Short Notes
This Repository will contain short notes on useful developer resources

---

## Valgrind
### Commands
* valgrind --leak-check=yes myprog arg1 arg2
* valgrind --log-file=gg --leak-check=full --show-leak-kinds=definite --error-limit=no --num-callers=20 --track-origins=yes myprog arg1 arg2

Links : 
* [Quick Start Guide](https://www.valgrind.org/docs/manual/quick-start.html#quick-start.interpret)

---

## GDB

|Use|Command|
|----------|-------------|
|Start GDB (with optional core dump)|gdb <program> [core dump]|
|Start GDB and pass arguments|gdb --args <program> <args…>|
|Start GDB and attach to process|gdb --pid <pid>|
|Run the program|run, r|
|Run the program with args|r arg1 arg2|
|Kill the running program|kill|
|Set a new breakpoint|break <function_name>|
|Set a new breakpoint|break <file:line_number>|
|Set a new breakpoint|break <line_number>|
|backtrace|backtrace, bt|
|Show call stack|where|
|Select the stack frame to operate on|frame <frame#>, f <frame#>|
|backtrace full|backtracefull|
|Show call stack, also print the local variables in each frame|where full|
|Go to next instruction (source line), diving into function|s,step |
|Go to next instruction (source line) but donʻt dive into functions|n,next|
|Quits gdb|q|
|break with conditions|br file.cpp:914 if strcmp(table_name,"asdasdasd")==0|
|Quits gdb|i thr|
|Print informations about the break- and watchpoints|info breakpoints, i br|
|Print the local variables in the currentlyselected stack frame|info locals|
|call function|call exit(0)|

* [Tutorial and examples](https://www.tutorialspoint.com/gnu_debugger/gdb_commands.htm)
* [Cheat Sheet](https://darkdust.net/files/GDB%20Cheat%20Sheet.pdf)  

---

## Git
### Commands
* [cheat sheet](file:///C:/Users/vikumw/Downloads/SWTM-2088_Atlassian-Git-Cheatsheet%20(1).pdf)
* git merge --no-ff  branchname
* git cherry-pick --abort
* git gc
git tag
* git tag -l "*1.0.20*"
Delete tag
* git tag -d <tag>
* git push origin :refs/tags/<tag>
Tag refresh
* git fetch --tags
Tag create and then push using
* git tag 
* git push origin refdata_1.0.22
* git revert --edit eb34beb90157c6f25c7aa44406d9f2abb29fc23f
* git add --patch <filename>
* git add .
* git log --pretty=oneline

---

## SQLPLUS
* sqlplus username/password@connect_identifier
* select <col1>,<col2> from <table>;

---

## GREP
* grep <options>  <pattern> <file or directory>
* grep -r  "ROUTING_SEQ" ./src/MainFrm.cpp
Get surrounding lines
* grep -r -c 10 "ROUTING_SEQ" ./src/MainFrm.cpp

---

## Linux File Search
* find ./ -iname "testFilename*"

