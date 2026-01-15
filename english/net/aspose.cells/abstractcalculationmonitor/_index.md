---
title: Class AbstractCalculationMonitor
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.AbstractCalculationMonitor class. Monitor for the user to track the progress of the formula calculation
type: docs
url: /net/aspose.cells/abstractcalculationmonitor/
---
## AbstractCalculationMonitor class

Monitor for the user to track the progress of the formula calculation.

```csharp
public abstract class AbstractCalculationMonitor
```

## Properties

| Name | Description |
| --- | --- |
| [CalculatedValue](../../aspose.cells/abstractcalculationmonitor/calculatedvalue/) { get; } | Gets the newly calculated value of the cell. Should be used only in [`AfterCalculate`](./aftercalculate/). |
| [OriginalValue](../../aspose.cells/abstractcalculationmonitor/originalvalue/) { get; } | Gets the old value of the calculated cell. Should be used only in [`BeforeCalculate`](./beforecalculate/) and [`AfterCalculate`](./aftercalculate/). |
| [ValueChanged](../../aspose.cells/abstractcalculationmonitor/valuechanged/) { get; } | Whether the cell's value has been changed after the calculation. Should be used only in [`AfterCalculate`](./aftercalculate/). |

## Methods

| Name | Description |
| --- | --- |
| virtual [AfterCalculate](../../aspose.cells/abstractcalculationmonitor/aftercalculate/)(int, int, int) | Implement this method to do business after one cell has been calculated. |
| virtual [BeforeCalculate](../../aspose.cells/abstractcalculationmonitor/beforecalculate/)(int, int, int) | Implement this method to do business before calculating one cell. |
| virtual [OnCircular](../../aspose.cells/abstractcalculationmonitor/oncircular/)(IEnumerator) | Implement this method to do business when calculating formulas with circular references. |

### Examples

```csharp
using Aspose.Cells;
using System;
using System.Collections;

namespace AsposeCellsExamples
{
    // Custom implementation of AbstractCalculationMonitor
    public class CustomCalculationMonitor : AbstractCalculationMonitor
    {
        public override void BeforeCalculate(int sheetIndex, int rowIndex, int colIndex)
        {
            Console.WriteLine($"Before calculating cell at Sheet: {sheetIndex}, Row: {rowIndex}, Column: {colIndex}");
        }

        public override void AfterCalculate(int sheetIndex, int rowIndex, int colIndex)
        {
            Console.WriteLine($"After calculating cell at Sheet: {sheetIndex}, Row: {rowIndex}, Column: {colIndex}");
            Console.WriteLine($"Original Value: {OriginalValue}, Calculated Value: {CalculatedValue}, Value Changed: {ValueChanged}");
        }

        public override bool OnCircular(IEnumerator circularCellsData)
        {
            Console.WriteLine("Circular reference detected.");
            return false; // Return false to stop calculation when circular reference is detected
        }
    }

    public class CalculationMonitorDemo
    {
        public static void RunDemo()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add some sample data
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].Formula = "=A1+A2";

            // Create an instance of CustomCalculationMonitor
            CustomCalculationMonitor monitor = new CustomCalculationMonitor();

            // Set calculation options
            CalculationOptions options = new CalculationOptions
            {
                CalculationMonitor = monitor,
                IgnoreError = false,
                Recursive = true
            };

            // Calculate formulas with the custom monitor
            workbook.CalculateFormula(options);

            // Save the workbook
            workbook.Save("CalculationMonitorDemo.xlsx");
            workbook.Save("CalculationMonitorDemo.pdf");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


