##ExternalConnection.SaveData
ExternalConnection property. True if the external data fetched over the connection to populate a table is to be saved with the workbook otherwise false
## ExternalConnection.SaveData property
True if the external data fetched over the connection to populate a table is to be saved with the workbook; otherwise, false.
```csharp
public bool SaveData { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
public class ExternalConnectionPropertySaveDataDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// Access the first external connection (assuming one exists)
ExternalConnection connection = workbook.DataConnections[0];
// Display the current SaveData value
Console.WriteLine("Initial SaveData value: " + connection.SaveData);
// Demonstrate setting the property (since it's read-write)
connection.SaveData = !connection.SaveData;
Console.WriteLine("Updated SaveData value: " + connection.SaveData);
// Save the workbook with the modified connection settings
workbook.Save("SaveDataDemo.xlsx");
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
