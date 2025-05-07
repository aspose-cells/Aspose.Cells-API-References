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
// Called: Console.WriteLine($"External Connection ID: {dataConn.ConnectionId}");
public static void Property_ConnectionId()
        {
            // Load an existing workbook that contains external connections
            Workbook workbook = new Workbook("ExternalConnectionCollectionExample_original.xlsx");

            // Get the external connection collection from the workbook
            ExternalConnectionCollection dataConns = workbook.DataConnections;

            // Iterate through the external connections and print their IDs
            for (int i = 0; i < dataConns.Count; i++)
            {
                ExternalConnection dataConn = dataConns[i];
                // Get external connection id
                Console.WriteLine($"External Connection ID: {dataConn.ConnectionId}");
            }

            // Example of accessing a specific external connection by ID
            int specificConnId = 1; // Example ID
            ExternalConnection specificConn = dataConns.GetExternalConnectionById(specificConnId);
            if (specificConn != null)
            {
                Console.WriteLine($"Found External Connection with ID {specificConnId}");
                // You can access and modify properties of the specific connection here
                specificConn.Name = "Updated Connection Name";
            }

            // Save the workbook if any changes were made
            workbook.Save("ExternalConnectionCollectionExample.xlsx");
        }
```

### See Also

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


