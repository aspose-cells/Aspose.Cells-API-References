---
title: QueryTable类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 1230
url: /zh/python-net/aspose.cells/querytable/
is_root: false
---
## QueryTable类
代表QueryTable信息。



QueryTable 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [connection_id](/cells/zh/python-net/aspose.cells/querytable/connection_id) |获取查询表的连接 ID。|
| [external_connection](/cells/zh/python-net/aspose.cells/querytable/external_connection) |获取相关的外部连接。|
| [name](/cells/zh/python-net/aspose.cells/querytable/name) |获取查询表的名称。|
| [result_range](/cells/zh/python-net/aspose.cells/querytable/result_range) |获取结果的范围。|
| [preserve_formatting](/cells/zh/python-net/aspose.cells/querytable/preserve_formatting) |返回或设置对象的 PreserveFormatting。|
| [adjust_column_width](/cells/zh/python-net/aspose.cells/querytable/adjust_column_width) |返回或设置对象的 AdjustColumnWidth。|



### 例子

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the first worksheet
worksheet = workbook.worksheets[0]
# Getting the first query table in the worksheet
qt = worksheet.query_tables[0]
# Getting display address of the query table.
address = qt.result_range.address

```

### 也可以看看
* 模块 [aspose.cells](..)
