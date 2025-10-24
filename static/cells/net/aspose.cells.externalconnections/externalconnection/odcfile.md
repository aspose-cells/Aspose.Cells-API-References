##ExternalConnection.OdcFile
ExternalConnection property. Specifies the full path to external connection file from which this connection was created. If a connection fails during an attempt to refresh data and reconnectionMethod1 then the spreadsheet application will try again using information from the external connection file instead of the connection object embedded within the workbook
## ExternalConnection.OdcFile property
Specifies the full path to external connection file from which this connection was created. If a connection fails during an attempt to refresh data, and reconnectionMethod=1, then the spreadsheet application will try again using information from the external connection file instead of the connection object embedded within the workbook.
```csharp
public string OdcFile { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
public class ExternalConnectionPropertyOdcFileDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// Access the first external connection (assuming one exists)
ExternalConnection connection = workbook.DataConnections[0];
// Display the current OdcFile value
Console.WriteLine("Initial OdcFile value: " + connection.OdcFile);
// Set a new OdcFile value (since it's read-write)
connection.OdcFile = @"C:\Connections\ExternalData.odc";
Console.WriteLine("Updated OdcFile value: " + connection.OdcFile);
// Clear the OdcFile value
connection.OdcFile = string.Empty;
Console.WriteLine("Cleared OdcFile value: " + connection.OdcFile);
// Save the workbook with the modified connection settings
workbook.Save("OdcFileDemo.xlsx");
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
