---
title: ExternalConnection.Id
second_title: Aspose.Cells for .NET API Reference
description: ExternalConnection property. Gets the id of the connection
type: docs
url: /net/aspose.cells.externalconnections/externalconnection/id/
---
## ExternalConnection.Id property

Gets the id of the connection.

```csharp
public int Id { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyIdDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            try
            {
                // Access the first external connection (workbook comes with default connections)
                ExternalConnection connection = workbook.DataConnections[0];

                // Display the current Id value (read-only property)
                Console.WriteLine("External Connection Id: " + connection.Id);

                // Display other read-only properties for context
                Console.WriteLine("Connection Class Type: " + connection.ClassType);
                Console.WriteLine("Connection Name: " + connection.Name);

                // Save the workbook
                workbook.Save("ExternalConnectionIdDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with connection Id: " + connection.Id);
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

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


