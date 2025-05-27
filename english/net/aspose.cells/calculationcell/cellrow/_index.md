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
using System;
using System.Collections;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationCellPropertyCellRowDemo
    {
        public static void Run()
        {
            // Create a workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data
            for (int row = 0; row < 10; row++)
            {
                for (int col = 0; col < 2; col++)
                {
                    worksheet.Cells[row, col].Formula = "=ROW()";
                }
            }

            // Calculate formulas
            workbook.CalculateFormula();

            // Process cells using CellRow property
            StringBuilder sb = new StringBuilder();
            IEnumerator enumerator = worksheet.Cells.GetEnumerator();
            
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                
                // Demonstrate CellRow usage - using cell.Row instead of CalculationCell
                if (cell.Row % 2 == 0)
                {
                    cell.PutValue("EVEN ROW");
                }
                else
                {
                    cell.PutValue("ODD ROW");
                }
                
                sb.AppendLine($"Cell {cell.Name} (Row {cell.Row}): {cell.StringValue}");
            }

            // Output results
            Console.WriteLine(sb.ToString());
        }
    }
}
```

### See Also

* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


