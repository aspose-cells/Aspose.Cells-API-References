##ExternalConnection.IsDeleted
ExternalConnection property. Indicates whether the associated workbook connection has been deleted. true if the connection has been deleted otherwise false
## ExternalConnection.IsDeleted property
Indicates whether the associated workbook connection has been deleted. true if the connection has been deleted; otherwise, false.
```csharp
public bool IsDeleted { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
public class ExternalConnectionPropertyIsDeletedDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// Access the first external connection (assuming one exists)
ExternalConnection connection = workbook.DataConnections[0];
// Display the initial IsDeleted value
Console.WriteLine("Initial IsDeleted value: " + connection.IsDeleted);
// Toggle the IsDeleted value (since it's read-write)
connection.IsDeleted = !connection.IsDeleted;
Console.WriteLine("Updated IsDeleted value: " + connection.IsDeleted);
// Save the workbook with the modified connection settings
workbook.Save("IsDeletedDemo.xlsx");
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
