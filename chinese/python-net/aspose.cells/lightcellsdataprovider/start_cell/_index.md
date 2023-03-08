---
title: start_cell方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 50
url: /zh/python-net/aspose.cells/lightcellsdataprovider/start_cell/
is_root: false
---
##  start_cell(cell) {#Cell}
开始保存一个单元格的数据。



```python
def start_cell(self, cell):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| cell | [Cell](/cells/zh/python-net/aspose.cells/cell) | Cell 用于填充数据的实施对象。它的列索引是最近调用[LightCellsDataProvider.next_cell()](/cells/zh/python-net/aspose.cells/lightcellsdataprovider/next_cell)的返回值。<br/>如果单元格已经在内部单元格模型中初始化，则将使用现有的单元格对象。<br/>否则将使用一个临时的 Cell 对象来实现填充数据。|
### 评论




### 也可以看看

* 模块 [aspose.cells](../../)
* 类 [LightCellsDataProvider](/cells/zh/python-net/aspose.cells/lightcellsdataprovider)
