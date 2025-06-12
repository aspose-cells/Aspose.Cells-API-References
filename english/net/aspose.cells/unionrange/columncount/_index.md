---
title: UnionRange.ColumnCount
second_title: Aspose.Cells for .NET API Reference
description: UnionRange property. Gets the count of rows in the range
type: docs
url: /net/aspose.cells/unionrange/columncount/
---
## UnionRange.ColumnCount property

Gets the count of rows in the range.

```csharp
public int ColumnCount { get; }
```

### Remarks

Only effects when it only contains one range.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyColumnCountDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Populate some data in the worksheet
            for (int i = 0; i < 5; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].Value = $"Cell {i},{j}";
                }
            }

            // Create a union range from A1 to E5
            Aspose.Cells.Range unionRange = worksheet.Cells.CreateRange("A1:E5");

            // Display the current ColumnCount value
            Console.WriteLine("Current ColumnCount of the range: " + unionRange.ColumnCount);

            // Note: ColumnCount is read-only, so we can't set it directly
            // To change the column count, we need to create a new range

            // Create a new range with different column count (A1:C5)
            Aspose.Cells.Range newRange = worksheet.Cells.CreateRange("A1:C5");
            Console.WriteLine("ColumnCount of new range: " + newRange.ColumnCount);

            // Demonstrate usage by checking if range contains data in all columns
            Console.WriteLine("Does original range have data in all columns? " + 
                (unionRange.ColumnCount == 5).ToString());
            Console.WriteLine("Does new range have data in all columns? " + 
                (newRange.ColumnCount == 5).ToString());

            // Save the workbook
            workbook.Save("UnionRangeColumnCountDemo.xlsx");
        }
    }
}
```

### See Also

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


