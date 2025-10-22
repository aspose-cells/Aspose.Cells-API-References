##DataModelConnection.Command
DataModelConnection property. The string containing the database command to pass to the data provider API that will interact with the external source in order to retrieve data
## DataModelConnection.Command property
The string containing the database command to pass to the data provider API that will interact with the external source in order to retrieve data
```csharp
public override string Command { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
using System.Runtime.Serialization;
public class DataModelConnectionPropertyCommandDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// Create DataModelConnection instance using uninitialized object
DataModelConnection connection = (DataModelConnection)FormatterServices.GetUninitializedObject(typeof(DataModelConnection));
((IList<ExternalConnection>)workbook.DataConnections).Add(connection);
// Display initial Command value (empty)
Console.WriteLine("Initial Command: " + connection.Command);
// Set the Command property
connection.Command = "SELECT * FROM Customers";
// Display the updated Command value
Console.WriteLine("Updated Command: " + connection.Command);
// Set other required properties for a complete connection
connection.CommandType = OLEDBCommandType.SqlStatement;
connection.ConnectionString = "Provider=SQLOLEDB;Data Source=Northwind;Integrated Security=SSPI";
// Save the workbook with the connection
workbook.Save("CommandDemo.xlsx");
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
* class [DataModelConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)
