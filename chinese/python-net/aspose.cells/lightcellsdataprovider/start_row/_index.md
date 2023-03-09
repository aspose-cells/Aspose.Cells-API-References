---
title: start_row方法
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 60
url: /zh/python-net/aspose.cells/lightcellsdataprovider/start_row/
is_root: false
---
##  start_row(row) {#Row}
开始保存一行数据。



```python
def start_row(self, row):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| row | [Row](/cells/zh/python-net/aspose.cells/row) |用于实现填充数据的Row对象，其行索引为最近调用[LightCellsDataProvider.next_row()](/cells/zh/python-net/aspose.cells/lightcellsdataprovider/next_row)的返回值。<br/>如果该行已在内部单元格模型中初始化，则将使用现有的行对象。<br/>否则将使用一个临时的 Row 对象来实现填充数据。|
### 评论

它将在开始保存一行及其单元格数据时调用。
如果当前行有一些自定义属性，如高度、样式等，
实现应在此处将这些属性设置为给定的 Row 对象。


### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [LightCellsDataProvider](/cells/zh/python-net/aspose.cells/lightcellsdataprovider)
