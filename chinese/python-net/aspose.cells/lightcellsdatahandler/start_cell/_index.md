---
title: start_cell方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 40
url: /zh/python-net/aspose.cells/lightcellsdatahandler/start_cell/
is_root: false
---
##  start_cell(column_index) {#int}
准备处理一个单元格。


### 返回

这个单元格是否需要处理。 false 忽略单元格并检查下一个单元格，直到到达当前行的单元格数据的末尾


```python
def start_cell(self, column_index):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| column_index | int |要处理的单元格的列索引|
### 评论

当到达当前行中的现有单元格时将调用它。当前行是 [LightCellsDataHandler.process_row(row)](/cells/zh/python-net/aspose.cells/lightcellsdatahandler/process_row) 最后一次调用的行。


### 也可以看看

* 模块 [aspose.cells](../../)
* 类 [LightCellsDataHandler](/cells/zh/python-net/aspose.cells/lightcellsdatahandler)
