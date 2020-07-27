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
* [Cheat Sheet](https://darkdust.net/files/GDB%20Cheat%20Sheet.pdf)
### Commands
| Tables   |      Are      |  Cool |
|----------|:-------------:|------:|
| col 1 is |  left-aligned | $1600 |
| col 2 is |    centered   |   $12 |
| col 3 is | right-aligned |    $1 |

* Start GDB (with optional core dump).gdb myprog core-myprog-10744-14748642800
* bt
* gdb myprog
* r arg1 arg2
* c
* bt
* d br
* i thr
* call exit(0)
* gdb myprog
* br Template::PrintTemplate()
* bt
* br file.cpp:37
* C
* S
* n
* br file.cpp:914 if strcmp(table_name,"asdasdasd")==0

---

## Git
### Commands
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

