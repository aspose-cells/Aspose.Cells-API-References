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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;

    public class CalculationCellPropertyCellDemo
    {
        public static void Run()
        {
            // Create a new workbook and get the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["B1"].Formula = "=A1*2";

            try
            {
                // Create CalculationCell instance using reflection since constructor is non-public
                CalculationCell calcCell = (CalculationCell)Activator.CreateInstance(
                    typeof(CalculationCell),
                    BindingFlags.NonPublic | BindingFlags.Instance,
                    null,
                    new object[] { workbook, worksheet, 0, 1, worksheet.Cells["B1"] },
                    null);

                // Display the Cell property value
                Console.WriteLine("Cell Name: " + calcCell.Cell.Name);
                Console.WriteLine("Cell Value: " + calcCell.Cell.Value);
                Console.WriteLine("Cell StringValue: " + calcCell.Cell.StringValue);
                Console.WriteLine("Cell Row: " + calcCell.Cell.Row);
                Console.WriteLine("Cell Column: " + calcCell.Cell.Column);
                Console.WriteLine("Cell IsFormula: " + calcCell.Cell.IsFormula);

                // Demonstrate related properties for context
                Console.WriteLine("CellRow: " + calcCell.CellRow);
                Console.WriteLine("CellColumn: " + calcCell.CellColumn);

                // Save the workbook
                workbook.Save("CellDemo.xlsx");
                Console.WriteLine("Cell property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [Cell](../../cell/)
* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


