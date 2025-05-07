---
title: ExternalConnectionCollection.GetExternalConnectionById
second_title: Aspose.Cells for .NET API Reference
description: ExternalConnectionCollection method. Gets the ExternalConnection element with the specified id
type: docs
url: /net/aspose.cells.externalconnections/externalconnectioncollection/getexternalconnectionbyid/
---
## ExternalConnectionCollection.GetExternalConnectionById method

Gets the [`ExternalConnection`](../../externalconnection/) element with the specified id.

```csharp
public ExternalConnection GetExternalConnectionById(int connId)
```

| Parameter | Type | Description |
| --- | --- | --- |
| connId | Int32 | external connection id |

### Return Value

The element with the specified id.

### Examples

```csharp
// Called: ExternalConnection specificConn = dataConns.GetExternalConnectionById(specificConnId);
public static void Method_Int32_()
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

* class [ExternalConnection](../../externalconnection/)
* class [ExternalConnectionCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


