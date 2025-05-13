---
title: ReferredArea.StartColumn
second_title: Aspose.Cells for .NET API Reference
description: ReferredArea property. The start column of the area
type: docs
url: /net/aspose.cells/referredarea/startcolumn/
---
## ReferredArea.StartColumn property

The start column of the area.

```csharp
public int StartColumn { get; }
```

### Examples

```csharp
// Called: int startCol = ra.StartColumn;
private void ReferredArea_Property_StartColumn(ReferredArea ra)
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


