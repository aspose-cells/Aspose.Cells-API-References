---
title: Cells.MoveRange
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Moves the range
type: docs
url: /net/aspose.cells/cells/moverange/
---
## Cells.MoveRange method

Moves the range.

```csharp
public void MoveRange(CellArea sourceArea, int destRow, int destColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceArea | CellArea | The range which should be moved. |
| destRow | Int32 | The dest row. |
| destColumn | Int32 | The dest column. |

### Examples

```csharp
// Called: cells.MoveRange(ca, 3, 1);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "TestMoveMergedCells_001.xls");
            CellArea ca = new CellArea();
            ca.StartRow = 1;
            ca.EndRow = 2;
            ca.StartColumn = 1;
            ca.EndColumn = 2;
            Cells cells = workbook.Worksheets[0].Cells;
            cells.MoveRange(ca, 3, 1);
            Assert.IsTrue(cells[3,1].IsMerged);
            workbook.Save(Constants.destPath + "TestMoveMergedCells_001.xls");
        }
```

### See Also

* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


