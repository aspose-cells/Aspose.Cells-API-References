---
title: WorksheetCollection.GetNamedRanges
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection method. Gets all predefined named ranges in the spreadsheet
type: docs
url: /net/aspose.cells/worksheetcollection/getnamedranges/
---
## WorksheetCollection.GetNamedRanges method

Gets all pre-defined named ranges in the spreadsheet.

```csharp
public Range[] GetNamedRanges()
```

### Return Value

An array of Range objects. If the defined Name's reference is external or has multiple ranges, no Range object will be returned for this Name.

Returns null if the named range does not exist.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetCollectionMethodGetNamedRangesDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Create some named ranges for demonstration
            worksheet.Cells.CreateRange("A1:B2").Name = "SalesData";
            worksheet.Cells.CreateRange("C3:D4").Name = "Expenses";

            try
            {
                // Call GetNamedRanges method to retrieve all named ranges
                Aspose.Cells.Range[] namedRanges = workbook.Worksheets.GetNamedRanges();

                // Display information about the named ranges
                Console.WriteLine("Found {0} named ranges:", namedRanges.Length);
                foreach (Aspose.Cells.Range range in namedRanges)
                {
                    Console.WriteLine("Name: {0}, Address: {1}", range.Name, range.Address);
                }

                // Save the workbook
                workbook.Save("GetNamedRangesDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetNamedRanges: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [Range](../../range/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


