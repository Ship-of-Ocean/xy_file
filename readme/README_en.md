# xy_file

- zh_CN [简体中文](readme/README_zh_CN.md)
- zh_TW [繁体中文](readme/README_zh_TW.md)
- en [English](readme/README_en.md)

If you think these tools are pretty good, Can you please have a cup of coffee?
![WeChat](readme/WeChat.png)
![Alipay](readme/Alipay.png)

## Description
Easy File tools, especially for regular.


## 安装

```
    pip install xy_file
```

## How to use

###### 1. Terminal
```
# Delete all py files under current work folder.
xy_file -w clean -g "*.py"

```

###### 2. python script

```
from xy_file.File import File
from pathlib import Path

touch_file_path = Path.cwd().joinpath("test.txt")
# create file if it not exists
file_path = File.touch(touch_file_path)
# if file_path is not empty, it means you created the file successful.
```


## Contact


```
Wechat: yuyangitt
Mail: 845262968@qq.com
```