---
title: Range.ClearContents
second_title: Aspose.Cells for .NET API Reference
description: Range method. Clears the contents of this range
type: docs
url: /net/aspose.cells/range/clearcontents/
---
## Range.ClearContents method

Clears the contents of this range.

```csharp
public void ClearContents()
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodClearContentsDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Populate some data in cells
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue(123);
            worksheet.Cells["A2"].PutValue(DateTime.Now);
            worksheet.Cells["B2"].PutValue("Test Value");

            // Get a range of cells
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2");

            try
            {
                // Display values before clearing
                Console.WriteLine("Before ClearContents:");
                for (int i = 0; i < range.RowCount; i++)
                {
                    for (int j = 0; j < range.ColumnCount; j++)
                    {
                        Console.Write(range[i, j].Value + "\t");
                    }
                    Console.WriteLine();
                }

                // Clear contents by setting Value to null
                range.Value = null;

                // Display values after clearing
                Console.WriteLine("\nAfter ClearContents:");
                for (int i = 0; i < range.RowCount; i++)
                {
                    for (int j = 0; j < range.ColumnCount; j++)
                    {
                        Console.Write(range[i, j].Value + "\t");
                    }
                    Console.WriteLine();
                }

                Console.WriteLine("ClearContents method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearContents method: {ex.Message}");
            }

            // Save the result
            workbook.Save("RangeMethodClearContentsDemo.xlsx");
        }
    }
}
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


