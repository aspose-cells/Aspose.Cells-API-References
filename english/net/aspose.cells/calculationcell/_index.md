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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Reflection;

    public class CellsClassCalculationCellDemo
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

                // Display basic properties
                Console.WriteLine($"Cell Row: {calcCell.CellRow}");
                Console.WriteLine($"Cell Column: {calcCell.CellColumn}");
                Console.WriteLine($"Cell Value: {calcCell.Cell.Value}");
                Console.WriteLine($"Workbook Name: {calcCell.Workbook.FileName}");
                Console.WriteLine($"Worksheet Name: {calcCell.Worksheet.Name}");

                // Save the workbook
                workbook.Save("CalculationCellDemo.xlsx");
                Console.WriteLine("CalculationCell demonstration completed successfully.");
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

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


