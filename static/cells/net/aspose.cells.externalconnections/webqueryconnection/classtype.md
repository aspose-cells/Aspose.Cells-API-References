##WebQueryConnection.ClassType
WebQueryConnection property. Gets the type of this ExternalConnection object
## WebQueryConnection.ClassType property
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
public class WebQueryConnectionPropertyClassTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// Access an existing web query connection or create one through proper initialization
if (workbook.DataConnections.Count > 0 &&
workbook.DataConnections[0] is WebQueryConnection connection)
{
// Display the ClassType value (read-only property)
Console.WriteLine("WebQueryConnection ClassType: " + connection.ClassType);
// Verify the expected enum value for web query
Console.WriteLine("Expected WebQuery enum value: " +
(connection.ClassType == ExternalConnectionClassType.WebQuery ? "Match" : "Mismatch"));
// Save the workbook
workbook.Save("WebQueryConnectionClassTypeDemo.xlsx");
}
else
{
Console.WriteLine("No web query connections found in the workbook.");
}
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
* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)
