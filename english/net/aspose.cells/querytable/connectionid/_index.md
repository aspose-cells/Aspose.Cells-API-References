---
title: QueryTable.ConnectionId
second_title: Aspose.Cells for .NET API Reference
description: QueryTable property. Gets the connection id of the query table
type: docs
url: /net/aspose.cells/querytable/connectionid/
---
## QueryTable.ConnectionId property

Gets the connection id of the query table.

```csharp
public int ConnectionId { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class QueryTablePropertyConnectionIdDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to simulate a query table scenario
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("Sample Data");

            try
            {
                // Check if there are any query tables in the worksheet
                if (worksheet.QueryTables.Count > 0)
                {
                    // Get the first query table
                    QueryTable queryTable = worksheet.QueryTables[0];

                    // Display the ConnectionId property value (read-only)
                    Console.WriteLine("Query Table ConnectionId: " + queryTable.ConnectionId);

                    // Display other related properties for context
                    Console.WriteLine("Query Table Name: " + queryTable.Name);
                    Console.WriteLine("External Connection: " +
                        (queryTable.ExternalConnection != null ? queryTable.ExternalConnection.Name : "None"));
                }
                else
                {
                    Console.WriteLine("No query tables found in the worksheet.");
                }

                // Save the workbook
                workbook.Save("ConnectionIdDemo.xlsx");
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


