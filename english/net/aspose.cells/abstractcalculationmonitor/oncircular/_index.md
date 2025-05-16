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
namespace AsposeCellsExamples.AbstractCalculationMonitorMethodOnCircularWithIEnumeratorDemo
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class AbstractCalculationMonitorMethodOnCircularWithIEnumeratorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create circular reference between A1 and B1
            worksheet.Cells["A1"].Formula = "B1";
            worksheet.Cells["B1"].Formula = "A1";

            // Create and assign custom calculation monitor
            CalculationOptions options = new CalculationOptions();
            options.CalculationMonitor = new CircularRefMonitor();

            try
            {
                workbook.CalculateFormula(options);
                Console.WriteLine("Formula calculation completed.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Calculation error: {ex.Message}");
            }

            workbook.Save("OnCircularDemo.xlsx");
        }
    }

    public class CircularRefMonitor : AbstractCalculationMonitor
    {
        public override bool OnCircular(IEnumerator circularCellsData)
        {
            Console.WriteLine("Processing circular references:");
            
            while (circularCellsData.MoveNext())
            {
                if (circularCellsData.Current is Cell cell)
                {
                    Console.WriteLine($"Found circular reference in cell {cell.Name}");
                    
                    // Add visual indicator for circular reference
                    Style style = cell.GetStyle();
                    style.Font.Color = System.Drawing.Color.Red;
                    cell.SetStyle(style);
                    
                    if (cell.Comment == null)
                    {
                        int commentIndex = cell.Worksheet.Comments.Add(cell.Name);
                        Comment comment = cell.Worksheet.Comments[commentIndex];
                        comment.Note = "Circular reference detected";
                        comment.Author = "System Monitor";
                    }
                }
            }
            
            return true; // Continue calculation
        }
    }
}
```

### See Also

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


