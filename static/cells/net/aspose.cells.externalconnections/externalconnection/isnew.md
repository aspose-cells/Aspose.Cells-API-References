##ExternalConnection.IsNew
ExternalConnection property. True if the connection has not been refreshed for the first time otherwise false. This state can happen when the user saves the file before a query has finished returning
## ExternalConnection.IsNew property
True if the connection has not been refreshed for the first time; otherwise, false. This state can happen when the user saves the file before a query has finished returning.
```csharp
public bool IsNew { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
public class ExternalConnectionPropertyIsNewDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// Access the first external connection (newly created connections are typically "IsNew")
ExternalConnection connection = workbook.DataConnections[0];
// Display the initial IsNew value
Console.WriteLine("Initial IsNew value: " + connection.IsNew);
// Since IsNew is read-write, demonstrate setting it
connection.IsNew = false;
Console.WriteLine("Updated IsNew value: " + connection.IsNew);
// Save the workbook with the modified connection settings
workbook.Save("IsNewDemo.xlsx");
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
