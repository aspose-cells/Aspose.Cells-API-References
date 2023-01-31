---
title: QueryTable class
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 1230
url: /python-net/aspose.cells/querytable/
is_root: false
---

## QueryTable class

Represents QueryTable information.



The QueryTable type exposes the following members:

### Properties
| Property | Description |
| :- | :- |
| [connection_id](/cells/python-net/aspose.cells/querytable/connection_id) | Gets the connection id of the query table. |
| [external_connection](/cells/python-net/aspose.cells/querytable/external_connection) | Gets the relate external connection. |
| [name](/cells/python-net/aspose.cells/querytable/name) | Gets the name of querytable. |
| [result_range](/cells/python-net/aspose.cells/querytable/result_range) | Gets the range of the result. |
| [preserve_formatting](/cells/python-net/aspose.cells/querytable/preserve_formatting) | Returns or sets the PreserveFormatting of the object. |
| [adjust_column_width](/cells/python-net/aspose.cells/querytable/adjust_column_width) | Returns or sets the AdjustColumnWidth of the object. |


### Example 


```
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
### See Also

* module [aspose.cells](../)
