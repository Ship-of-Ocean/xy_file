# xy_file

- zh_CN [简体中文](readme/README_zh_CN.md)
- zh_TW [繁体中文](readme/README_zh_TW.md)
- en [English](readme/README_en.md)

## 說明
簡單檔操作工具，特殊功能為不同路徑匹配規則的添加。


## 安裝

```
    pip install git+https://github.com/Ship-of-Ocean/xy_file.git --user
```

## 使用

###### 1. 命令行
```
# 刪除目前的目錄下所有 py 文稿檔
xy_file -w clean -g "*.py"

```

###### 2. python腳本

```
from xy_file.File import File
from pathlib import Path

touch_file_path = Path.cwd().joinpath("test.txt")
# 創建檔案當該檔案路徑為空
file_path = File.touch(touch_file_path)
# 如果file_path不為空 說明創建空檔成功
```