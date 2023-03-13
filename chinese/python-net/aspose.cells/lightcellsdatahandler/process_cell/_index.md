---
title: process_cell方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 20
url: /zh/python-net/aspose.cells/lightcellsdatahandler/process_cell/
is_root: false
---
##  process_cell(cell) {#Cell}
开始处理一个细胞。


### 返回

此单元格是否需要保留在当前工作表的单元格模型中。
一般应该为false，这样所有的cell在处理后都不会保存在内存中，然后保存内存。
对于某些特殊目的，例如用户需要在处理完整个工作簿后稍后访问某些单元格，
用户可以使此方法返回 true 以将这些特殊单元格保留在 Cells 模型中，并在以后通过 API 访问它们，例如 Cells[行，列]。
但是，将单元格数据保留在 Cells 模型中将需要更多内存，如果保留所有单元格则读取模板文件
在 LightCells 模式下将变得与以正常方式阅读相同。


```python
def process_cell(self, cell):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| cell | [Cell](/cells/zh/python-net/aspose.cells/cell) | Cell 当前正在处理的对象|
### 评论

读取一个单元格的数据后将调用它。


### 也可以看看

* 模块 [aspose.cells](../../)
* 类 [LightCellsDataHandler](/cells/zh/python-net/aspose.cells/lightcellsdatahandler)
