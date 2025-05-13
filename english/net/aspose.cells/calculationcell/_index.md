---
title: Class CalculationCell
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.CalculationCell class. Represents the calculation relevant data about one cell which is being calculated
type: docs
url: /net/aspose.cells/calculationcell/
---
## CalculationCell class

Represents the calculation relevant data about one cell which is being calculated.

```csharp
public class CalculationCell
```

## Properties

| Name | Description |
| --- | --- |
| [Cell](../../aspose.cells/calculationcell/cell/) { get; } | Gets the Cell object which is being calculated. |
| [CellColumn](../../aspose.cells/calculationcell/cellcolumn/) { get; } | Gets the column index of the cell. |
| [CellRow](../../aspose.cells/calculationcell/cellrow/) { get; } | Gets the row index of the cell. |
| [Workbook](../../aspose.cells/calculationcell/workbook/) { get; } | Gets the Workbook object. |
| [Worksheet](../../aspose.cells/calculationcell/worksheet/) { get; } | Gets the Worksheet object where the cell is in. |

## Methods

| Name | Description |
| --- | --- |
| [SetCalculatedValue](../../aspose.cells/calculationcell/setcalculatedvalue/)(object) | Sets the calculated value for the cell. |

### Remarks

All objects provided by this class are for "read" purpose only. User should not change any data in the Workbook during the formula calculation process, Otherwise unexpected result or Exception may be caused.

### Examples

```csharp
// Called: CalculationCell cc = (CalculationCell)circularCellsData.Current;
public static void Cells_Type_CalculationCell(IEnumerator circularCellsData, TextWriter writer)
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

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


