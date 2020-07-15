# Developer Short Notes
This Repository will contain short notes on useful developer resources

## Valgrind
### Commands
* valgrind --leak-check=yes myprog arg1 arg2
* valgrind --log-file=gg --leak-check=full --show-leak-kinds=definite --error-limit=no --num-callers=20 --track-origins=yes myprog arg1 arg2

Links : 
* [Quick Start Guide](https://www.valgrind.org/docs/manual/quick-start.html#quick-start.interpret)

## GDB
### Commands
---
* gdb myprog core-myprog-10744-14748642800
* bt
---
* gdb myprog
* r arg1 arg2
---
* c
* bt
* d br
* i thr
* call exit(0)
---
* gdb myprog
* br Template::PrintTemplate()
* bt
* br file.cpp:37
* C
* S
* n
---
* br file.cpp:914 if strcmp(table_name,"asdasdasd")==0
---
