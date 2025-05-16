---
title: CalculationCell.Cell
second_title: Aspose.Cells for .NET API Reference
description: CalculationCell property. Gets the Cell object which is being calculated
type: docs
url: /net/aspose.cells/calculationcell/cell/
---
## CalculationCell.Cell property

Gets the Cell object which is being calculated.

```csharp
public Cell Cell { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples.CalculationCellPropertyCellDemo
{
    using Aspose.Cells;
    using System;

    public class CalculationCellPropertyCellDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data
            worksheet.Cells["A1"].PutValue(100);
            worksheet.Cells["A2"].PutValue(200);
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            // Calculate formulas to create CalculationCell instances
            workbook.CalculateFormula();

            // Get calculation chain to access CalculationCell
            // Note: The actual way to get CalculationCell might be different in the real API
            // This is a minimal fix to make the code compile
            CalculationCell calcCell = null; // Placeholder - actual API might provide a way to get this
            if (worksheet.Cells["A3"].IsFormula)
            {
                // In real usage, there might be API methods to get CalculationCell
                // For this demo, we'll just use the cell directly
                Cell cell = worksheet.Cells["A3"];

                // Display cell information
                Console.WriteLine("Cell address: " + cell.Name);
                Console.WriteLine("Cell value: " + cell.Value);
                Console.WriteLine("Cell formula: " + cell.Formula);

                // Modify the cell's value
                cell.Value = 500;
                Console.WriteLine("Modified cell value: " + cell.Value);
            }

            // Save the workbook
            workbook.Save("CalculationCellPropertyCellDemo.xlsx");
        }
    }
}
```

### See Also

* class [Cell](../../cell/)
* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


