## Check version

```
$ docker run --rm -i -t -v $(pwd):/source topher515/prolog-swi:apt swipl --version
SWI-Prolog version 6.6.4 for amd64
```

## Compile Hello, World

```
$ docker run --rm -i -t -v $(pwd):/source topher515/prolog-swi swipl -s  /source/hello_world.pl
% /source/hello_world.pl compiled 0.00 sec, 3 clauses
Hello World
```

## Run REPL

```
$ docker run --rm -i -t topher515/prolog-swi:apt swipl
Welcome to SWI-Prolog (Multi-threaded, 64 bits, Version 6.6.4)
Copyright (c) 1990-2013 University of Amsterdam, VU Amsterdam
SWI-Prolog comes with ABSOLUTELY NO WARRANTY. This is free software,
and you are welcome to redistribute it under certain conditions.
Please visit http://www.swi-prolog.org for details.

For help, use ?- help(Topic). or ?- apropos(Word).

?-
```