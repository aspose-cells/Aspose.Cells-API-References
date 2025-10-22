##DBConnection.ClassType
DBConnection property. Gets the type of this ExternalConnection object
## DBConnection.ClassType property
Gets the type of this [`ExternalConnection`](../../externalconnection/) object.
```csharp
public override ExternalConnectionClassType ClassType { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
public class DBConnectionPropertyClassTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// Create a new DBConnection instance by adding it to the collection
// Since DBConnection doesn't have a public parameterless constructor,
// we'll let the collection create it for us
var connections = workbook.DataConnections;
DBConnection dbConnection = (DBConnection)connections[connections.Count];
// Display the ClassType value (read-only property)
Console.WriteLine("DBConnection ClassType: " + dbConnection.ClassType);
// Demonstrate setting other properties to make the example more meaningful
dbConnection.ConnectionString = "Server=myServerAddress;Database=myDataBase;";
dbConnection.CommandType = OLEDBCommandType.TableName;
dbConnection.Command = "Customers";
// Save the workbook
workbook.Save("DBConnectionDemo.xlsx");
Console.WriteLine("ClassType demonstration completed successfully.");
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
* enum [ExternalConnectionClassType](../../externalconnectionclasstype/)
* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)
