##ExternalConnection.SourceFile
ExternalConnection property. Used when the external data source is filebased. When a connection to such a data source fails the spreadsheet application attempts to connect directly to this file. May be expressed in URI or systemspecific file path notation
## ExternalConnection.SourceFile property
Used when the external data source is file-based. When a connection to such a data source fails, the spreadsheet application attempts to connect directly to this file. May be expressed in URI or system-specific file path notation.
```csharp
public string SourceFile { get; set; }
```
### Examples
```csharp
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
namespace AsposeCellsExamples
{
public class ExternalConnectionPropertySourceFileDemo
{
public static void Run()
{
Workbook workbook = new Workbook("input.xlsx");
ExternalConnectionCollection connections = workbook.DataConnections;
foreach (ExternalConnection connection in connections)
{
if (!string.IsNullOrEmpty(connection.SourceFile))
connection.SourceFile = connection.SourceFile.Replace("C:\\", "D:\\");
}
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)
