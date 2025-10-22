##ExternalConnectionCollection.Item
ExternalConnectionCollection property. Gets the ExternalConnection element at the specified index
## ExternalConnectionCollection indexer (1 of 2)
Gets the [`ExternalConnection`](../../externalconnection/) element at the specified index.
```csharp
public ExternalConnection this[int index] { get; set; }
```
| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |
### Return Value
The element at the specified index.
### See Also
* class [ExternalConnection](../../externalconnection/)
* class [ExternalConnectionCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)
## ExternalConnectionCollection indexer (2 of 2)
Gets the [`ExternalConnection`](../../externalconnection/) element with the specified name.
```csharp
public ExternalConnection this[string connectionName] { get; }
```
| Parameter | Description |
| --- | --- |
| connectionName | the name of data connection |
### Return Value
The element with the specified name.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
public class ExternalConnectionCollectionPropertyItemDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// Access the external connections collection
ExternalConnectionCollection connections = workbook.DataConnections;
// Add a sample connection (if needed for demonstration)
// This assumes the collection allows adding connections
// connections.Add(new ExternalConnection());
// Demonstrate accessing an item by name (read operation)
// Note: In a real scenario, you would need actual connection names
if (connections.Count > 0)
{
// Get first connection name (if available)
string connectionName = connections[0].Name;
// Access the Item property
ExternalConnection connection = connections[connectionName];
// Display connection information
Console.WriteLine($"Connection Name: {connection.Name}");
Console.WriteLine($"Connection Type: {connection.Type}");
}
else
{
Console.WriteLine("No external connections available to demonstrate Item property");
}
// Save the workbook
workbook.Save("ExternalConnectionDemo.xlsx");
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
* class [ExternalConnection](../../externalconnection/)
* class [ExternalConnectionCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)
