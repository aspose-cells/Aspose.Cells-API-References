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
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassCalculationCellDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("=A1+A2");

            // Calculate formulas
            workbook.CalculateFormula();

            // Get cell reference for A3
            Cell cell = worksheet.Cells["A3"];

            // Output cell information
            Console.WriteLine($"Worksheet: {worksheet.Name}");
            Console.WriteLine($"Cell: A3");
            Console.WriteLine($"Value: {cell.Value}");
            Console.WriteLine($"Calculated Value: {cell.StringValue}");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


