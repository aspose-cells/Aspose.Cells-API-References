---
title: Cells.HideRow
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Hides a row
type: docs
url: /net/aspose.cells/cells/hiderow/
---
## Cells.HideRow method

Hides a row.

```csharp
public void HideRow(int row)
```

| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index. |

### Examples

```csharp
// Called: cells.HideRow(-1);
[Test, Ignore("Not ready to test this yet")]
        public void Method_Int32_()
        {
            caseName = "testHideRow_Exception_001";
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells.HideRow(-1);
            string msg = message + "cells.HideRow(-1)";
            writeToExcel(caseName, msg);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


