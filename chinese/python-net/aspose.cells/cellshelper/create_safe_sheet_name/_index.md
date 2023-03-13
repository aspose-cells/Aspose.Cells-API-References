---
title: create_safe_sheet_name方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 90
url: /zh/python-net/aspose.cells/cellshelper/create_safe_sheet_name/
is_root: false
---
##  create_safe_sheet_name(name_proposal) {#str}
检查给定的工作表名称并在需要时创建有效的工作表名称。
如果给定的工作表名称符合excel工作表名称的规则，则返回它。
否则，如果长度超过限制，字符串将被截断
无效字符将被替换为' '，然后返回重建的字符串值。


### 返回




```python
def create_safe_sheet_name(self, name_proposal):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| name_proposal | str |要使用的工作表名称|


##  create_safe_sheet_name(name_proposal, replace_char) {#str-char}
检查给定的工作表名称并在需要时创建有效的工作表名称。
如果给定的工作表名称符合excel工作表名称的规则，则返回它。
否则，如果长度超过限制，字符串将被截断
无效的字符将被替换为给定的字符，然后返回重建的字符串值。


### 返回




```python
def create_safe_sheet_name(self, name_proposal, replace_char):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| name_proposal | str |要使用的工作表名称|
| replace_char | char |将用于替换给定工作表名称中的无效字符的字符|



### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [CellsHelper](/cells/zh/python-net/aspose.cells/cellshelper)
