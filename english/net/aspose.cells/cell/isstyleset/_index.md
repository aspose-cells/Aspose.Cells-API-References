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
// Called: testAreEqual(false, cells[row, col].IsStyleSet, caseName);
private void Property_IsStyleSet(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            for (int row = 10; row &lt;= 14; row++)
            {
                for (int col = 0; col &lt;= 3; col++)
                {
                    testAreEqual(false, cells[row, col].IsStyleSet, caseName);
                }
            }
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


