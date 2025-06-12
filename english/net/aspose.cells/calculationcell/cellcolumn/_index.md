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
using System;
using Aspose.Cells;
using System.IO;
using System.Collections;

namespace AsposeCellsExamples
{
    public class CalculationCellPropertyCellColumnDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            // Calculate formulas
            workbook.CalculateFormula();

            // Get the calculation chain
            IEnumerator enumerator = workbook.Worksheets.GetEnumerator();
            while (enumerator.MoveNext())
            {
                Worksheet ws = (Worksheet)enumerator.Current;
                foreach (Cell cell in ws.Cells)
                {
                    if (cell.IsFormula)
                    {
                        // Demonstrate CellColumn property usage
                        string cellAddress = CellsHelper.ColumnIndexToName(cell.Column) + (cell.Row + 1);
                        Console.WriteLine($"Calculated cell at {cellAddress} in sheet '{ws.Name}'");
                        Console.WriteLine($"Value: {cell.Value}");
                    }
                }
            }
        }
    }
}
```

### See Also

* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


