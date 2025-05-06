---
title: Cells.UnhideColumn
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Unhides a column
type: docs
url: /net/aspose.cells/cells/unhidecolumn/
---
## Cells.UnhideColumn method

Unhides a column

```csharp
public void UnhideColumn(int column, double width)
```

| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | Column index. |
| width | Double | Column width. |

### Examples

```csharp
// Called: cells.UnhideColumn(2, -1);
[Test]
        public void Method_Double_()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells.HideColumn(2);
            cells.UnhideColumn(2, -1);
            Assert.AreEqual(cells.Columns[2].Width, cells.StandardWidth);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


