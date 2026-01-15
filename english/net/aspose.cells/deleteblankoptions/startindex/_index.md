---
title: DeleteBlankOptions.StartIndex
second_title: Aspose.Cells for .NET API Reference
description: DeleteBlankOptions property. Specifies the start row/column index of the range to check and delete blank row/column
type: docs
url: /net/aspose.cells/deleteblankoptions/startindex/
---
## DeleteBlankOptions.StartIndex property

Specifies the start row/column index of the range to check and delete blank row/column.

```csharp
public int StartIndex { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyStartIndexDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Populate some cells with values
            cells[2, 0].PutValue("Row 3");
            cells[5, 0].PutValue("Row 6");
            cells[9, 0].PutValue("Row 10");

            Console.WriteLine("Before deleting blank rows:");
            for (int i = 0; i <= 10; i++)
            {
                Console.WriteLine($"Row {i + 1}: {(cells[i, 0].Value ?? "empty")}");
            }

            // Delete blank rows starting from index 4 (Row 5) to index 7 (Row 8)
            DeleteBlankOptions options = new DeleteBlankOptions();
            options.StartIndex = 4;
            options.EndIndex = 7;
            cells.DeleteBlankRows(options);

            Console.WriteLine("\nAfter deleting blank rows from Row 5 to Row 8:");
            for (int i = 0; i <= 7; i++)
            {
                Console.WriteLine($"Row {i + 1}: {(cells[i, 0].Value ?? "empty")}");
            }
        }
    }
}
```

### See Also

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


