---
title: freeze_panes方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 120
url: /zh/python-net/aspose.cells/worksheet/freeze_panes/
is_root: false
---
##  freeze_panes(cell_name, freezed_rows, freezed_columns) {#str-int-int}
冻结工作表中指定单元格的窗格。



```python
def freeze_panes(self, cell_name, freezed_rows, freezed_columns):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| cell_name | str | Cell 名称。|
| freezed_rows | int |顶部窗格中的可见行数，不超过行索引。|
| freezed_columns | int |左窗格中可见的列数，不超过列索引。|
### 评论

行索引和列索引不能都为零。行数和列数
也不能全为零。

##  freeze_panes(row, column, freezed_rows, freezed_columns) {#int-int-int-int}
冻结工作表中指定单元格的窗格。



```python
def freeze_panes(self, row, column, freezed_rows, freezed_columns):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| row | int |行索引。|
| column | int |列索引。|
| freezed_rows | int |顶部窗格中的可见行数，不超过行索引。|
| freezed_columns | int |左窗格中可见的列数，不超过列索引。|
### 评论

行索引和列索引不能都为零。行数和列数
也不能全为零。


前两个参数指定冻结位置，后两个参数指定左上窗格中的冻结区域。


### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Worksheet](/cells/zh/python-net/aspose.cells/worksheet)
