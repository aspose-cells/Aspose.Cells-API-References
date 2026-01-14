---
title: AbstractCalculationMonitor.OnCircular
second_title: Aspose.Cells for .NET API Reference
description: AbstractCalculationMonitor method. Implement this method to do business when calculating formulas with circular references
type: docs
url: /net/aspose.cells/abstractcalculationmonitor/oncircular/
---
## AbstractCalculationMonitor.OnCircular method

Implement this method to do business when calculating formulas with circular references.

```csharp
public virtual bool OnCircular(IEnumerator circularCellsData)
```

| Parameter | Type | Description |
| --- | --- | --- |
| circularCellsData | IEnumerator | IEnumerator with [`CalculationCell`](../../calculationcell/) items representing cells that depend on circular references. |

### Return Value

Whether the formula engine needs to calculate those cells in circular after this call. True to let the formula engine continue to do calculation for them. False to let the formula engine just mark those cells as Calculated.

### Remarks

In the implementation user may also set the expected value as calculated result for part/all of those cells so the formula engine will not calculate them recursively.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class AbstractCalculationMonitorMethodOnCircularDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create a circular reference scenario
            worksheet.Cells["A1"].Formula = "=B1";
            worksheet.Cells["B1"].Formula = "=A1";

            CalculationOptions options = new CalculationOptions();
            options.CalculationMonitor = new CircularReferenceMonitor();

            try
            {
                workbook.CalculateFormula(options);
                Console.WriteLine("Calculation completed. Check console for circular reference handling.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Calculation error: {ex.Message}");
            }

            workbook.Save("OnCircularDemo.xlsx");
        }

        private class CircularReferenceMonitor : AbstractCalculationMonitor
        {
            public override bool OnCircular(IEnumerator circularCellsData)
            {
                Console.WriteLine("Circular reference detected!");
                while (circularCellsData.MoveNext())
                {
                    Console.WriteLine($"Circular cell: {circularCellsData.Current}");
                }
                return true; // Continue calculation
            }
        }
    }
}
```

### See Also

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


