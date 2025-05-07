---
title: ReferredArea.SheetName
second_title: Aspose.Cells for .NET API Reference
description: ReferredArea property. Indicates which sheet this reference is in
type: docs
url: /net/aspose.cells/referredarea/sheetname/
---
## ReferredArea.SheetName property

Indicates which sheet this reference is in.

```csharp
public string SheetName { get; }
```

### Remarks

If it references to multiple worksheets, the returned value is just like the range expression in the formula. For example "Sheet1:Sheet3" for the reference in formula "=SUM(Sheet1:Sheet3!$A$1:$B$2)".

### Examples

```csharp
// Called: Cells cells = _wb.Worksheets[ra.SheetName].Cells;
private void Property_SheetName(ReferredArea ra)
            {
                if (ra.IsExternalLink)
                {
                    Console.WriteLine("External link is not supported.");
                    return;
                }
                Cells cells = _wb.Worksheets[ra.SheetName].Cells;
                int startRow = ra.StartRow;
                int startCol = ra.StartColumn;
                int endRow = ra.EndRow;
                int endCol = ra.EndColumn;
                for (int i = startRow; i <= endRow; i++)
                {
                    for (int j = startCol; j <= endCol; j++)
                    {
                        Cell cell = cells.CheckCell(i, j);
                        if (cell == null)
                        {
                            Console.WriteLine(CellsHelper.CellIndexToName(i, j) + ": cell is null");
                        }
                        else
                        {
                            Console.WriteLine(cell.Name + ".Value: " + cell.Value);
                        }
                    }
                }
            }
```

### See Also

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


