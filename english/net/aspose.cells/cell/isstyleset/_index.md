---
title: Cell.IsStyleSet
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Indicates if the cells style is set. If return false it means this cell has a default cell format
type: docs
url: /net/aspose.cells/cell/isstyleset/
---
## Cell.IsStyleSet property

Indicates if the cell's style is set. If return false, it means this cell has a default cell format.

```csharp
public bool IsStyleSet { get; }
```

### Examples

```csharp
// Called: testAreEqual(false, cells[5, 2].IsStyleSet, caseName);
private void Cell_Property_IsStyleSet(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            for (int row = 3; row <= 4; row++)
            {
                for (int col = 2; col <= 3; col++)
                {
                    checkStyle(cells[row, col].GetStyle());
                }
            }
            testAreEqual(false, cells[5, 2].IsStyleSet, caseName);
            testAreEqual(false, cells[5, 3].IsStyleSet, caseName);
            checkRowStyle(cells[7, 0].GetStyle());
            for (int col = 1; col <= 4; col++)
            {
                testAreEqual(false, cells[7, col].IsStyleSet, caseName);
            }
            checkRowStyle(cells[7, 6].GetStyle());
            checkRowStyle(cells[7, 7].GetStyle());
            checkRowStyle(cells[7, 87].GetStyle());
            checkRowStyle(cells[7, 120].GetStyle());
            checkRowStyle(cells[7, 201].GetStyle());
            checkRowStyle(cells[7, 255].GetStyle());
            checkColumnStyle(cells.Columns[5].GetStyle());
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


