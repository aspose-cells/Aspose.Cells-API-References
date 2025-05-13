---
title: PivotTable.TableRange2
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Returns a CellArea object that represents the range containing the entire PivotTable report includes page fields. Readonly
type: docs
url: /net/aspose.cells.pivot/pivottable/tablerange2/
---
## PivotTable.TableRange2 property

Returns a CellArea object that represents the range containing the entire PivotTable report, includes page fields. Read-only.

```csharp
public CellArea TableRange2 { get; }
```

### Examples

```csharp
// Called: CellArea ca1 = pt1.TableRange2;
internal static  void PivotTable_Property_TableRange2(Worksheet s1, Worksheet s2,bool f)
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

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


