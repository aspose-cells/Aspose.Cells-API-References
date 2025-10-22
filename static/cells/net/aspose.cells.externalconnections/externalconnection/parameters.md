##ExternalConnection.Parameters
ExternalConnection property. Gets ConnectionParameterCollection for an ODBC or web query
## ExternalConnection.Parameters property
Gets [`ConnectionParameterCollection`](../../connectionparametercollection/) for an ODBC or web query.
```csharp
public ConnectionParameterCollection Parameters { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using System;
public class ExternalConnectionPropertyParametersDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// Access the first external connection (assuming one exists)
ExternalConnection connection = workbook.DataConnections[0];
// Display the Parameters collection information
ConnectionParameterCollection parameters = connection.Parameters;
Console.WriteLine($"Number of parameters: {parameters.Count}");
// Display each parameter's information if available
foreach (ConnectionParameter param in parameters)
{
Console.WriteLine($"Parameter name: {param.Name}");
Console.WriteLine($"Parameter type: {param.Type}");
Console.WriteLine($"Parameter prompt: {param.Prompt}");
Console.WriteLine("----------------------");
}
// Save the workbook
workbook.Save("ParametersDemo.xlsx");
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
* class [ConnectionParameterCollection](../../connectionparametercollection/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)
