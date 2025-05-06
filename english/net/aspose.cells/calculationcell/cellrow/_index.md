---
title: CalculationCell.CellRow
second_title: Aspose.Cells for .NET API Reference
description: CalculationCell property. Gets the row index of the cell
type: docs
url: /net/aspose.cells/calculationcell/cellrow/
---
## CalculationCell.CellRow property

Gets the row index of the cell.

```csharp
public int CellRow { get; }
```

### Examples

```csharp
// Called: writer.Write(sheet.Name + &amp;quot;!&amp;quot; + CellsHelper.ColumnIndexToName(cc.CellColumn) + (cc.CellRow + 1));
public static void Property_CellRow(IEnumerator circularCellsData, TextWriter writer)
        {
            circularCellsData.MoveNext();
            CalculationCell cc = (CalculationCell)circularCellsData.Current;
            Worksheet sheet = cc.Worksheet;
            writer.Write(sheet.Name + &quot;!&quot; + CellsHelper.ColumnIndexToName(cc.CellColumn) + (cc.CellRow + 1));
            writer.Flush();
            while (circularCellsData.MoveNext())
            {
                writer.Write(&quot;-&gt;&quot;);
                cc = (CalculationCell)circularCellsData.Current;
                if (cc.Worksheet != sheet)
                {
                    sheet = cc.Worksheet;
                    writer.Write(sheet.Name + &quot;!&quot;);
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


