---
title: Workbook.DataConnections
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Gets the ExternalConnection collection
type: docs
url: /net/aspose.cells/workbook/dataconnections/
---
## Workbook.DataConnections property

Gets the [`ExternalConnection`](../../../aspose.cells.externalconnections/externalconnection/) collection.

```csharp
public ExternalConnectionCollection DataConnections { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookPropertyDataConnectionsDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Create a sample worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to make the example meaningful
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Access the DataConnections property
                var dataConnections = workbook.DataConnections;

                // Display the current value of the property (read operation)
                Console.WriteLine("DataConnections count: " + dataConnections.Count);

                // Iterate through the connections if any exist
                for (int i = 0; i < dataConnections.Count; i++)
                {
                    var connection = dataConnections[i];
                    Console.WriteLine($"Connection {i + 1}: {connection.Name}");
                }

                // Show how the property affects behavior
                Console.WriteLine("DataConnections has been demonstrated");

                // Save the result
                workbook.Save("DataConnectionsDemo.xlsx");
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

* class [ExternalConnectionCollection](../../../aspose.cells.externalconnections/externalconnectioncollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


