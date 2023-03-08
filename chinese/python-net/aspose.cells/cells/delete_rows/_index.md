---
title: delete_rows方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 260
url: /zh/python-net/aspose.cells/cells/delete_rows/
is_root: false
---
##  delete_rows(row_index, total_rows) {#int-int}
删除多行。



```python
def delete_rows(self, row_index, total_rows):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| row_index | int |要删除的第一行索引。|
| total_rows | int |要删除的行数。|
### 评论

如果删除的范围包含表（ListObject）的顶部（不是全部），
范围不能被删除，什么也不会做。它像 MS Excel 一样工作。

##  delete_rows(row_index, total_rows, update_reference) {#int-int-bool}
删除工作表中的多行。


### 返回




```python
def delete_rows(self, row_index, total_rows, update_reference):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| row_index | int |行索引。|
| total_rows | int |要删除的行数。|
| update_reference | bool |指示是否更新其他工作表中的引用。|



### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Cells](/cells/zh/python-net/aspose.cells/cells)
