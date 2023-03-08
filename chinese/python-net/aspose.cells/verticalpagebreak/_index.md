---
title: VerticalPageBreak类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 1560
url: /zh/python-net/aspose.cells/verticalpagebreak/
is_root: false
---
##  VerticalPageBreak类
封装表示垂直分页符的对象。



VerticalPageBreak 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [start_row](/cells/zh/python-net/aspose.cells/verticalpagebreak/start_row) |获取垂直分页符的起始行索引。|
| [end_row](/cells/zh/python-net/aspose.cells/verticalpagebreak/end_row) |获取垂直分页符的结束行索引。|
| [column](/cells/zh/python-net/aspose.cells/verticalpagebreak/column) |获取垂直分页符的列索引。|



### 例子

```python
from aspose.cells import Workbook

excel = Workbook()
# Add a pagebreak at G5
excel.worksheets[0].horizontal_page_breaks.add("G5")
excel.worksheets[0].vertical_page_breaks.add("G5")

```

### 也可以看看
* 模块 [aspose.cells](..)
