---
title: Cells.HideColumn
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Hides a column
type: docs
url: /net/aspose.cells/cells/hidecolumn/
---
## Cells.HideColumn method

Hides a column.

```csharp
public void HideColumn(int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | Column index. |

### Examples

```csharp
// Called: cells.HideColumn(0);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells.HideColumn(0);
            cells.HideRow(0);
            Assert.AreEqual(1, workbook.Worksheets[0].FirstVisibleRow);
            Assert.AreEqual(1, workbook.Worksheets[0].FirstVisibleColumn);
            workbook.Save(Constants.destPath + "CELLSJAVA42631.xlsx");
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


