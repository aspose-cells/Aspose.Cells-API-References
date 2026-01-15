---
title: QueryTable.ResultRange
second_title: Aspose.Cells for .NET API Reference
description: QueryTable property. Gets the range of the result
type: docs
url: /net/aspose.cells/querytable/resultrange/
---
## QueryTable.ResultRange property

Gets the range of the result.

```csharp
public Range ResultRange { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTablePropertyResultRangeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to simulate a query table
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");

            try
            {
                // Check if there are any query tables in the worksheet
                if (worksheet.QueryTables.Count > 0)
                {
                    // Get the first query table
                    QueryTable queryTable = worksheet.QueryTables[0];

                    // Display the ResultRange property value (read-only operation)
                    Aspose.Cells.Range resultRange = queryTable.ResultRange;
                    Console.WriteLine("ResultRange Address: " + resultRange.Address);
                    Console.WriteLine("ResultRange Row Count: " + resultRange.RowCount);
                    Console.WriteLine("ResultRange Column Count: " + resultRange.ColumnCount);
                    Console.WriteLine("ResultRange First Row: " + resultRange.FirstRow);
                    Console.WriteLine("ResultRange First Column: " + resultRange.FirstColumn);

                    // Display the values in the result range
                    Console.WriteLine("Values in ResultRange:");
                    foreach (Cell cell in resultRange)
                    {
                        Console.WriteLine($"Cell [{cell.Row}, {cell.Column}]: {cell.Value}");
                    }
                }
                else
                {
                    Console.WriteLine("No query tables found in the worksheet.");
                }

                // Save the workbook
                workbook.Save("ResultRangeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [Range](../../range/)
* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


