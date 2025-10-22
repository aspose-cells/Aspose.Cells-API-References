##ExternalConnection.Name
ExternalConnection property. Specifies the name of the connection. Each connection must have a unique name
## ExternalConnection.Name property
Specifies the name of the connection. Each connection must have a unique name.
```csharp
public string Name { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
namespace AsposeCellsExamples
{
public class ExternalConnectionPropertyNameDemo
{
public static void Run()
{
Workbook workbook = new Workbook("example.xlsm");
foreach (ExternalConnection connection in workbook.DataConnections)
{
Console.WriteLine("Connection Name: " + connection.Name);
}
workbook.Save("output.xlsm");
}
}
}
```
### See Also
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)
