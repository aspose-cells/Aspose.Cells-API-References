##ExternalConnection.SecondCommand
ExternalConnection property. Specifies a second command text string that is persisted when PivotTable serverbased page fields are in use. For ODBC connections serverCommand is usually a broader query than command no WHERE clause is present in the former. Based on these 2 commandsCommand and ServerCommand parameter UI can be populated and parameterized queries can be constructed
## ExternalConnection.SecondCommand property
Specifies a second command text string that is persisted when PivotTable server-based page fields are in use. For ODBC connections, serverCommand is usually a broader query than command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed
```csharp
public virtual string SecondCommand { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
public class ExternalConnectionPropertySecondCommandDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// Access the first external connection (assuming one exists)
ExternalConnection connection = workbook.DataConnections[0];
// Display the current SecondCommand value (read operation)
Console.WriteLine("Initial SecondCommand value: " + connection.SecondCommand);
// Set a new SecondCommand value (since it's read-write)
connection.SecondCommand = "SELECT * FROM Customers WHERE Country = 'USA'";
Console.WriteLine("Updated SecondCommand value: " + connection.SecondCommand);
// Clear the SecondCommand to demonstrate setting empty string
connection.SecondCommand = string.Empty;
Console.WriteLine("Cleared SecondCommand value: " + connection.SecondCommand);
// Save the workbook with the modified connection settings
workbook.Save("SecondCommandDemo.xlsx");
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
