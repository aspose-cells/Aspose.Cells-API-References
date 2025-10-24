##ExternalConnection.SSOId
ExternalConnection property. Identifier for Single Sign On SSO used for authentication between an intermediate spreadsheetML server and the external data source
## ExternalConnection.SSOId property
Identifier for Single Sign On (SSO) used for authentication between an intermediate spreadsheetML server and the external data source.
```csharp
public string SSOId { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
public class ExternalConnectionPropertySSOIdDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// Access the first external connection
ExternalConnection connection = workbook.DataConnections[0];
// Display initial SSOId value (likely null for new connection)
Console.WriteLine("Initial SSOId value: " + connection.SSOId);
// Set a new SSOId value (since it's read-write)
connection.SSOId = "sso-12345";
Console.WriteLine("Updated SSOId value: " + connection.SSOId);
// Clear the SSOId
connection.SSOId = null;
Console.WriteLine("Cleared SSOId value: " + connection.SSOId);
// Save the workbook with the modified connection settings
workbook.Save("SSOIdDemo.xlsx");
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
