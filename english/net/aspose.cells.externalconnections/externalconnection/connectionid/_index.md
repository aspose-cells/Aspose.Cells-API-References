---
title: ExternalConnection.ConnectionId
second_title: Aspose.Cells for .NET API Reference
description: ExternalConnection property. Specifies The unique identifier of this connection
type: docs
url: /net/aspose.cells.externalconnections/externalconnection/connectionid/
---
## ExternalConnection.ConnectionId property

Specifies The unique identifier of this connection.

```csharp
[Obsolete("Use ExternalConnection.Id property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int ConnectionId { get; }
```

### Remarks

NOTE: This property is now obsolete. Instead, please use ExternalConnection.Id property. This property will be removed 12 months later since October 2024. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyConnectionIdDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            try
            {
                // Access the first external connection (workbook comes with default connections)
                ExternalConnection connection = workbook.DataConnections[0];

                // Display the ConnectionId value (read-only property)
                Console.WriteLine("ConnectionId value: " + connection.ConnectionId);

                // Display the Id value for comparison (also read-only)
                Console.WriteLine("Id value: " + connection.Id);

                // Show that both properties are read-only by attempting to display them
                Console.WriteLine("ConnectionId and Id are both read-only properties");
                Console.WriteLine("ConnectionId: " + connection.ConnectionId + ", Id: " + connection.Id);

                // Save the workbook
                workbook.Save("ConnectionIdDemo.xlsx");
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


