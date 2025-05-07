---
title: CellArea.StartRow
second_title: Aspose.Cells for .NET API Reference
description: CellArea field. Gets or set the start row of this area
type: docs
url: /net/aspose.cells/cellarea/startrow/
---
## CellArea.StartRow field

Gets or set the start row of this area.

```csharp
public int StartRow;
```

### Examples

```csharp
// Called: Aspose.Cells.Range r2 = s2.Cells.CreateRange(ca1.StartRow, ca1.StartColumn, ca1.EndRow - ca1.StartRow + 1, ca1.EndColumn - ca1.StartColumn + 1);
internal static  void Field_StartRow(Worksheet s1, Worksheet s2,bool f)
        {
            for (int j = 0; j < s1.PivotTables.Count; j++)
            {
                PivotTable pt1 = s1.PivotTables[j];
                PivotTable pt2 = s2.PivotTables[j];
                CellArea ca1 = pt1.TableRange2;
                CellArea ca2 = pt2.TableRange2;
                Aspose.Cells.Range r1 = s1.Cells.CreateRange(ca1.StartRow, ca1.StartColumn, ca1.EndRow - ca1.StartRow + 1, ca1.EndColumn - ca1.StartColumn + 1);
                Aspose.Cells.Range r2 = s2.Cells.CreateRange(ca1.StartRow, ca1.StartColumn, ca1.EndRow - ca1.StartRow + 1, ca1.EndColumn - ca1.StartColumn + 1);
                RangeUtil.Compare(r1, r2, f);
            }
        }
```

### See Also

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


