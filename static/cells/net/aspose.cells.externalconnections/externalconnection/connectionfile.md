##ExternalConnection.ConnectionFile
ExternalConnection property. Gets the connection file
## ExternalConnection.ConnectionFile property
Gets the connection file.
```csharp
public virtual string ConnectionFile { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
namespace AsposeCellsExamples
{
public class ExternalConnectionPropertyConnectionFileDemo
{
public static void Run()
{
Workbook workbook = new Workbook("example.xlsx");
ExternalConnection conn = workbook.Worksheets[0].PivotTables[0].GetSourceDataConnections()[0];
Console.WriteLine("ConnectionFile: " + conn.ConnectionFile);
workbook.Save("output.xlsx");
Workbook reloadedWorkbook = new Workbook("output.xlsx");
ExternalConnection reloadedConn = reloadedWorkbook.Worksheets[0].PivotTables[0].GetSourceDataConnections()[0];
Console.WriteLine("ConnectionFile after reload: " + reloadedConn.ConnectionFile);
}
}
}
```
### See Also
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)
