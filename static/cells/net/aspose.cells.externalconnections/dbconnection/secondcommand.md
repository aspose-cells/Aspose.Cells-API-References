##DBConnection.SecondCommand
DBConnection property. Specifies a second command text string that is persisted when PivotTable serverbased page fields are in use. For ODBC connections serverCommand is usually a broader query than command no WHERE clause is present in the former. Based on these 2 commandsCommand and ServerCommand parameter UI can be populated and parameterized queries can be constructed
## DBConnection.SecondCommand property
Specifies a second command text string that is persisted when PivotTable server-based page fields are in use. For ODBC connections, serverCommand is usually a broader query than command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed
```csharp
public override string SecondCommand { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
public class DBConnectionPropertySecondCommandDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// Create a new DBConnection instance by adding it to the collection
var connections = workbook.DataConnections;
DBConnection dbConnection = (DBConnection)connections[0];
// Set up a basic connection
dbConnection.ConnectionString = "Server=myServer;Database=myDB;";
dbConnection.CommandType = OLEDBCommandType.SqlStatement;
dbConnection.Command = "SELECT * FROM Customers WHERE Country = 'USA'";
// Set and demonstrate the SecondCommand property
dbConnection.SecondCommand = "SELECT * FROM Customers";
Console.WriteLine("SecondCommand value: " + dbConnection.SecondCommand);
// Modify the SecondCommand to show it's writable
dbConnection.SecondCommand = "SELECT * FROM Orders";
Console.WriteLine("Updated SecondCommand value: " + dbConnection.SecondCommand);
// Save the workbook
workbook.Save("SecondCommandDemo.xlsx");
Console.WriteLine("SecondCommand demonstration completed successfully.");
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
* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)
