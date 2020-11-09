# bash-utils

```bash
$ git clone https://github.com/zx80live/bash-utils
$ cd ./bash-utils

```



### util_text

```bash
# import util_text
$ source util_text
```



```bash
$ strformats
```



![image-20201109202710823](https://raw.githubusercontent.com/zx80live/zx80live.github.io/master/img/bash-utils/strformats_example_1.png)

```bash
$ strformat "Hello, World" CYAN BOLD ITALIC
```

![image-20201109203059108](https://raw.githubusercontent.com/zx80live/zx80live.github.io/master/img/bash-utils/strformat_example_1.png)

```bash
$ strlen "Hello, World"
12
```

```bash
$ substring "r" 10 3
ABC
```

```bash
$ strdrop_right "0123456789ABCDEFGH" 8
0123456789
```

```bash
$ strdrop_left "0123456789ABCDEFGH" 10
ABCDEFGH
```

```bash
$ strfill_right "ABC" '.' 10
ABC..........
```

```bash
$ strfill_left "ABC" '.' 10
..........ABC
```

```bash
$ strdecorate "some text" '~~' '~~'
~~some text~~
```

```bash
# get matched regex groups
$ strregex "Some string with some 123 number and SPECIAL word." '.*([0-9]{3}).*(SPECIAL).*'
Some string with some 123 number and SPECIAL word.
123
SPECIAL
```

```bash
$ strunwrap "~~some text~~" '~~' '~~'
some text
```

```bash
$ strtake_left "0123456789ABCDEFGH" 5
01234
```

```bash
$ strtake_right "0123456789ABCDEFGH" 5
DEFGH
```

```bash
$ strsplit 'A.B.C.D' '.'
A
B
C
D
```
