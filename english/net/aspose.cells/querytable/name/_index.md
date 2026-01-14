---
title: QueryTable.Name
second_title: Aspose.Cells for .NET API Reference
description: QueryTable property. Gets the name of querytable
type: docs
url: /net/aspose.cells/querytable/name/
---
## QueryTable.Name property

Gets the name of querytable.

```csharp
public string Name { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTablePropertyNameDemo
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

                    // Display the Name property value (read-only operation)
                    Console.WriteLine("Query Table Name: " + queryTable.Name);

                    // Display other read-only properties for context
                    Console.WriteLine("Connection ID: " + queryTable.ConnectionId);
                    Console.WriteLine("Result Range: " + queryTable.ResultRange.Address);
                }
                else
                {
                    Console.WriteLine("No query tables found in the worksheet.");
                }

                // Save the workbook
                workbook.Save("QueryTableNameDemo.xlsx");
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

* class [QueryTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


