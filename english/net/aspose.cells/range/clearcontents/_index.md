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

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data to demonstrate clearing
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            worksheet.Cells["A2"].PutValue("Sample");
            worksheet.Cells["B2"].PutValue("Data");

            try
            {
                // Create a range covering cells A1:B2
                Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2");

                // Display the range contents before clearing
                Console.WriteLine("Before clearing:");
                Console.WriteLine($"A1: {worksheet.Cells["A1"].Value}");
                Console.WriteLine($"B1: {worksheet.Cells["B1"].Value}");
                Console.WriteLine($"A2: {worksheet.Cells["A2"].Value}");
                Console.WriteLine($"B2: {worksheet.Cells["B2"].Value}");

                // Call ClearContents to remove all values in the range
                range.ClearContents();

                // Display the range contents after clearing
                Console.WriteLine("\nAfter clearing:");
                Console.WriteLine($"A1: {worksheet.Cells["A1"].Value}");
                Console.WriteLine($"B1: {worksheet.Cells["B1"].Value}");
                Console.WriteLine($"A2: {worksheet.Cells["A2"].Value}");
                Console.WriteLine($"B2: {worksheet.Cells["B2"].Value}");

                // Save the workbook
                workbook.Save("ClearContentsDemo.xlsx");
                Console.WriteLine("\nWorkbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


