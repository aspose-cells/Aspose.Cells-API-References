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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;

    public class CalculationCellPropertyWorksheetDemo
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

                // Display the Worksheet property value
                Console.WriteLine("Worksheet Name: " + calcCell.Worksheet.Name);
                Console.WriteLine("Worksheet Index: " + calcCell.Worksheet.Index);
                Console.WriteLine("Worksheet Type: " + calcCell.Worksheet.Type);

                // Demonstrate other related properties
                Console.WriteLine("Cell Row: " + calcCell.CellRow);
                Console.WriteLine("Cell Column: " + calcCell.CellColumn);

                // Save the workbook
                workbook.Save("WorksheetDemo.xlsx");
                Console.WriteLine("Worksheet property demonstration completed successfully.");
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

* class [Worksheet](../../worksheet/)
* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


