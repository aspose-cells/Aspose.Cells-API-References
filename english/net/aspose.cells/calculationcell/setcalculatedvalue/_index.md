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
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationCellMethodSetCalculatedValueWithObjectDemo
    {
        public static void Run()
        {
            // Create a workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create cells and set formulas
            worksheet.Cells[0, 0].Formula = "=1";
            worksheet.Cells[1, 0].Formula = "=2";
            worksheet.Cells[2, 0].Formula = "=3";

            // Calculate formulas
            workbook.CalculateFormula();

            // Get cells and set calculated values directly
            Cell cell1 = worksheet.Cells[0, 0];
            Cell cell2 = worksheet.Cells[1, 0];
            Cell cell3 = worksheet.Cells[2, 0];

            // Set calculated values with different object types
            cell1.Value = 101; // Integer
            cell2.Value = "Test Value"; // String
            cell3.Value = DateTime.Now; // DateTime

            // Output the results
            Console.WriteLine("Cell A1 calculated value: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("Cell A2 calculated value: " + worksheet.Cells["A2"].Value);
            Console.WriteLine("Cell A3 calculated value: " + worksheet.Cells["A3"].Value);
        }
    }
}
```

### See Also

* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


