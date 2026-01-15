---
title: CalculationCell.SetCalculatedValue
second_title: Aspose.Cells for .NET API Reference
description: CalculationCell method. Sets the calculated value for the cell
type: docs
url: /net/aspose.cells/calculationcell/setcalculatedvalue/
---
## CalculationCell.SetCalculatedValue method

Sets the calculated value for the cell.

```csharp
public void SetCalculatedValue(object v)
```

### Remarks

User can set the calculated result by this method to ignore the automatic calculation for the cell.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;

    public class CalculationCellMethodSetCalculatedValueWithObjectDemo
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

                // Set a calculated value using the SetCalculatedValue method
                calcCell.SetCalculatedValue(42); // Using an integer value as the Object parameter

                // Display information about the cell
                Console.WriteLine("Cell Row: " + calcCell.CellRow);
                Console.WriteLine("Cell Column: " + calcCell.CellColumn);
                Console.WriteLine("SetCalculatedValue method called successfully with value: 42");

                // Save the workbook
                workbook.Save("SetCalculatedValueDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetCalculatedValue: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


