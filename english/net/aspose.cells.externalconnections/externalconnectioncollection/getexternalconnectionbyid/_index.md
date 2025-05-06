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
            Workbook workbook = new Workbook(&quot;ExternalConnectionCollectionExample_original.xlsx&quot;);

            // Get the external connection collection from the workbook
            ExternalConnectionCollection dataConns = workbook.DataConnections;

            // Iterate through the external connections and print their IDs
            for (int i = 0; i &lt; dataConns.Count; i++)
            {
                ExternalConnection dataConn = dataConns[i];
                // Get external connection id
                Console.WriteLine($&quot;External Connection ID: {dataConn.ConnectionId}&quot;);
            }

            // Example of accessing a specific external connection by ID
            int specificConnId = 1; // Example ID
            ExternalConnection specificConn = dataConns.GetExternalConnectionById(specificConnId);
            if (specificConn != null)
            {
                Console.WriteLine($&quot;Found External Connection with ID {specificConnId}&quot;);
                // You can access and modify properties of the specific connection here
                specificConn.Name = &quot;Updated Connection Name&quot;;
            }

            // Save the workbook if any changes were made
            workbook.Save(&quot;ExternalConnectionCollectionExample.xlsx&quot;);
        }
```

### See Also

* class [ExternalConnection](../../externalconnection/)
* class [ExternalConnectionCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


