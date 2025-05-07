---
title: Cells.GetLastDataRow
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Gets the last row index of cell which contains data in the specified column
type: docs
url: /net/aspose.cells/cells/getlastdatarow/
---
## Cells.GetLastDataRow method

Gets the last row index of cell which contains data in the specified column.

```csharp
public int GetLastDataRow(int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | Column index. |

### Return Value

last row index.

### Examples

```csharp
// Called: Assert.AreEqual(cells.GetLastDataRow(0), 3);
[Test]
        public void Method_Int32_()
        { 
            Workbook wb = new Workbook(Constants.sourcePath + "NET53695.xlsx");
            Cells cells = wb.Worksheets[0].Cells;
            Assert.AreEqual(cells.GetLastDataRow(0), 3);
            Assert.AreEqual(cells.GetLastDataRow(1), 7);
            Assert.AreEqual(cells.GetLastDataRow(2), 9);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


