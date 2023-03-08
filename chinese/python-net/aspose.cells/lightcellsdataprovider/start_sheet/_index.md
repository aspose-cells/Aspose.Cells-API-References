---
title: start_sheet方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 70
url: /zh/python-net/aspose.cells/lightcellsdataprovider/start_sheet/
is_root: false
---
##  start_sheet(sheet_index) {#int}
开始保存工作表。


### 返回

如果此提供者将为给定工作表提供数据，则为真；如果给定工作表应使用其正常数据模型 (Cells)，则为 false。


```python
def start_sheet(self, sheet_index):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| sheet_index | int |要保存的当前工作表的索引。|
### 评论

在保存工作簿的过程中，将在保存工作表开始时调用。
如果提供商需要参考*`sheetIndex`*之后
在 startRow(Row) 或 startCell(Cell) 方法中，
也就是说，如果流程需要知道正在处理哪个工作表，
实施应保留*`sheetIndex`*这里的价值。


### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [LightCellsDataProvider](/cells/zh/python-net/aspose.cells/lightcellsdataprovider)
