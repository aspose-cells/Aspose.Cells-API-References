##DataModelConnection.ConnectionString
DataModelConnection property. The connection information string is used to make contact with an OLE DB or ODBC data source
## DataModelConnection.ConnectionString property
The connection information string is used to make contact with an OLE DB or ODBC data source.
```csharp
public override string ConnectionString { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
using System.Runtime.Serialization;
public class DataModelConnectionPropertyConnectionStringDemo
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
// Display initial ConnectionString value (empty)
Console.WriteLine("Initial ConnectionString: " + connection.ConnectionString);
// Set the ConnectionString property
connection.ConnectionString = "Provider=SQLOLEDB;Data Source=Northwind;Integrated Security=SSPI";
// Display the updated ConnectionString value
Console.WriteLine("Updated ConnectionString: " + connection.ConnectionString);
// Set other required properties for a complete connection
connection.Command = "SELECT * FROM Customers";
connection.CommandType = OLEDBCommandType.SqlStatement;
// Save the workbook with the connection
workbook.Save("ConnectionStringDemo.xlsx");
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
