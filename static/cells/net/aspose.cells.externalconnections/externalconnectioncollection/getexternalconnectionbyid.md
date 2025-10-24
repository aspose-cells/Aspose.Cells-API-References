##ExternalConnectionCollection.GetExternalConnectionById
ExternalConnectionCollection method. Gets the ExternalConnection element with the specified id
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
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
namespace AsposeCellsExamples
{
public class ExternalConnectionCollectionMethodGetExternalConnectionByIdWithInt32Demo
{
public static void Run()
{
// Create a new workbook with sample data connections
Workbook workbook = new Workbook();
// Get the external connection collection
ExternalConnectionCollection dataConns = workbook.DataConnections;
// Create and add connections using proper API methods
// Note: In real usage, you would typically get existing connections
// rather than creating new ones this way
int connectionId1 = 1;
int connectionId2 = 2;
// Get specific connection by ID (will be null initially)
ExternalConnection specificConn = dataConns.GetExternalConnectionById(connectionId1);
if (specificConn == null)
{
Console.WriteLine($"No connection found with ID {connectionId1}");
// In real usage, you would work with existing connections
// or create them through proper API methods
}
else
{
Console.WriteLine($"Found connection: ID={specificConn.ConnectionId}, Name={specificConn.Name}");
specificConn.Name = "ModifiedConnection";
}
// Save the workbook
workbook.Save("ExternalConnectionDemo.xlsx");
}
}
}
```
### See Also
* class [ExternalConnection](../../externalconnection/)
* class [ExternalConnectionCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)
