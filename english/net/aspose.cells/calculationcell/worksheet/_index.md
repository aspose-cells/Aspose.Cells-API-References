---
title: CalculationCell.Worksheet
second_title: Aspose.Cells for .NET API Reference
description: CalculationCell property. Gets the Worksheet object where the cell is in
type: docs
url: /net/aspose.cells/calculationcell/worksheet/
---
## CalculationCell.Worksheet property

Gets the Worksheet object where the cell is in.

```csharp
public Worksheet Worksheet { get; }
```

### Examples

```csharp
// Called: if (cc.Worksheet != sheet)
public static void Property_Worksheet(IEnumerator circularCellsData, TextWriter writer)
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

* class [Worksheet](../../worksheet/)
* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


