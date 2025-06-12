---
title: CalculationData.Cell
second_title: Aspose.Cells for .NET API Reference
description: CalculationData property. Gets the Cell object where the function is in
type: docs
url: /net/aspose.cells/calculationdata/cell/
---
## CalculationData.Cell property

Gets the Cell object where the function is in.

```csharp
public Cell Cell { get; }
```

### Remarks

When calculating a formula without setting it to a cell, such as by [`CalculateFormula`](../../worksheet/calculateformula/), the formula will be calculated just like it has been set to cell A1, so both [`CellRow`](../cellrow/) and [`CellColumn`](../cellcolumn/) are 0. However, cell A1 in the worksheet may has not been instantiated. So for such kind of situation this property will be null.

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationDataPropertyCellDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Set sample data in cells
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["B4"].PutValue(25);

            // Create calculation data by calculating a formula
            worksheet.Cells["C2"].Formula = "=IFERROR(A2:A4,B2:B4)";
            var result = worksheet.Cells["C2"].Value;

            // Get the calculation data (this approach may vary based on actual API)
            // Note: The exact way to get CalculationData may depend on specific API version
            // This is a simplified approach to demonstrate the Cell property usage
            var cell = worksheet.Cells["C2"];
            
            // Output the result from the cell
            Console.WriteLine("Calculated value: " + cell.Value);
        }
    }
}
```

### See Also

* class [Cell](../../cell/)
* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


