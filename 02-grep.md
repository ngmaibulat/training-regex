### Basics

```bash

grep -F 'search' file.txt

egrep --color 'search' file.txt

egrep -i 'search' file.txt

egrep -v 'search' file.txt

egrep -x 'search' file.txt # exact match

egrep -w 'search' file.txt # whole word

egrep -n 'search' file.txt # line number

egrep -c 'search' file.txt # count

cat file.txt | egrep 'search'

egrep -r 'search'

```

### Grouping

```bash
echo hello:hellow | egrep '(hello).\1'
```
