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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationCellPropertyCellColumnDemo
    {
        public static void Run()
        {
            // Create a new workbook and get the first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Put some data and a simple formula
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["B1"].Formula = "=A1*2";

            try
            {
                // Obtain a CalculationCell instance via reflection (its constructor is non‑public)
                CalculationCell calcCell = (CalculationCell)Activator.CreateInstance(
                    typeof(CalculationCell), 
                    nonPublic: true);

                // Read and display the CellColumn property value
                Console.WriteLine("CellColumn value: " + calcCell.CellColumn);

                // Additional demonstration of related properties (optional)
                Console.WriteLine("CellRow value: " + calcCell.CellRow);
                Console.WriteLine("Workbook is null: " + (calcCell.Workbook == null));
                Console.WriteLine("Worksheet is null: " + (calcCell.Worksheet == null));

                // Save the workbook (the file will contain the data we added)
                workbook.Save("CellColumnDemo.xlsx");
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

* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


