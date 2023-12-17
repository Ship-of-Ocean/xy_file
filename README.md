# xy_file


## 安装

```
    git clone https://github.com/Ship-of-Ocean/xy_file.git
    cd xy_file
    python setup.py install
```

## 使用

###### 1. 命令行
```
# 删除当前目录下所有 py 脚本文件
xy_file -w clean -g "*.py"

```

###### 2. python脚本

```
from xy_file.File import File
from pathlib import Path

touch_file_path = Path.cwd().joinpath("test.txt")
# 创建文件当该文件路径为空
file_path = File.touch(touch_file_path)
# 如果file_path不为空 说明创建空文件成功
```