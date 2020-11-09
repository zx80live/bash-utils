# bash-utils

```bash
$ git clone https://github.com/zx80live/bash-utils
$ cd ./bash-utils

```

### util_files

```bash
# import util_files
$ source util_files
```

```bash
# create nested dirs if it isn't exist
$ touch_dir '/a/b/c/d/e/f'
```

```bash
# create file if it isn't exist including all nested dirs in its path
$ touch_file '/a/b/c/d/e/f/hello.txt'
```

### util_logs

```bash
# import util_logs
$ source util_logs
```

```bash
$ log_info 'some log info string'
```

![image-20201109210636121](https://raw.githubusercontent.com/zx80live/zx80live.github.io/master/img/bash-utils/log_info_example_1.png)

```bash
$ log_err 'some err string'
```

![image-20201109210744075](https://raw.githubusercontent.com/zx80live/zx80live.github.io/master/img/bash-utils/log_err_example_1.png)

```bash
$ log_debug 'some debug string'
# there is nothing in output, because log_level variable is LOG_LEVEL_INFO by default

$ export log_level=$LOG_LEVEL_DEBUG
$ log_debug 'some debug string'
```

![image-20201109211020220](https://raw.githubusercontent.com/zx80live/zx80live.github.io/master/img/bash-utils/log_debug_example_1.png)

### util_text

```bash
# import util_text
$ source util_text
```

```bash
# list of available formats
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
$ substring "0123456789ABCDEFGH" 10 3
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
