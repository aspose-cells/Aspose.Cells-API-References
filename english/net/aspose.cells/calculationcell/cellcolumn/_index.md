---
title: CalculationCell.CellColumn
second_title: Aspose.Cells for .NET API Reference
description: CalculationCell property. Gets the column index of the cell
type: docs
url: /net/aspose.cells/calculationcell/cellcolumn/
---
## CalculationCell.CellColumn property

Gets the column index of the cell.

```csharp
public int CellColumn { get; }
```

### Examples

```csharp
// Called: writer.Write(sheet.Name + "!" + CellsHelper.ColumnIndexToName(cc.CellColumn) + (cc.CellRow + 1));
public static void CalculationCell_Property_CellColumn(IEnumerator circularCellsData, TextWriter writer)
        {
            circularCellsData.MoveNext();
            CalculationCell cc = (CalculationCell)circularCellsData.Current;
            Worksheet sheet = cc.Worksheet;
            writer.Write(sheet.Name + "!" + CellsHelper.ColumnIndexToName(cc.CellColumn) + (cc.CellRow + 1));
            writer.Flush();
            while (circularCellsData.MoveNext())
            {
                writer.Write("->");
                cc = (CalculationCell)circularCellsData.Current;
                if (cc.Worksheet != sheet)
                {
                    sheet = cc.Worksheet;
                    writer.Write(sheet.Name + "!");
                }
                writer.Write(CellsHelper.ColumnIndexToName(cc.CellColumn) + (cc.CellRow + 1));
                writer.Flush();
            }
            writer.WriteLine();
        }
```

### See Also

* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


