---
title: UnionRange.GetEnumerator
second_title: Aspose.Cells for .NET API Reference
description: UnionRange method. Gets the enumerator for cells in this Range
type: docs
url: /net/aspose.cells/unionrange/getenumerator/
---
## UnionRange.GetEnumerator method

Gets the enumerator for cells in this Range.

```csharp
public IEnumerator GetEnumerator()
```

### Return Value

The cells enumerator

### Remarks

When traversing elements by the returned Enumerator, the cells collection should not be modified(such as operations that will cause new Cell/Row be instantiated or existing Cell/Row be deleted). Otherwise the enumerator may not be able to traverse all cells correctly(some elements may be traversed repeatedly or skipped).

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class UnionRangeMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Populate some data in cells
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(1.8);
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B4"].PutValue(3.2);

            // Create a range (changed from CreateUnionRange to CreateRange)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B4");

            try
            {
                // Get the enumerator for cells in the range
                IEnumerator enumerator = range.GetEnumerator();
                
                Console.WriteLine("Contents of the range:");
                while (enumerator.MoveNext())
                {
                    Cell cell = (Cell)enumerator.Current;
                    Console.WriteLine($"Cell {cell.Name}: {cell.Value}");
                }

                // Show range information
                Console.WriteLine($"\nRange Info - FirstRow: {range.FirstRow}, FirstColumn: {range.FirstColumn}");
                Console.WriteLine($"RowCount: {range.RowCount}, ColumnCount: {range.ColumnCount}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetEnumerator method: {ex.Message}");
            }
            
            // Save the workbook
            workbook.Save("UnionRangeGetEnumeratorDemo.xlsx");
        }
    }
}
```

### See Also

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


