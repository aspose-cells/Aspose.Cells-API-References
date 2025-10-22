##DBConnection.SeverCommand
DBConnection property. Specifies a second command text string that is persisted when PivotTable serverbased page fields are in use. For ODBC connections serverCommand is usually a broader query than command no WHERE clause is present in the former. Based on these 2 commandsCommand and ServerCommand parameter UI can be populated and parameterized queries can be constructed
## DBConnection.SeverCommand property
Specifies a second command text string that is persisted when PivotTable server-based page fields are in use. For ODBC connections, serverCommand is usually a broader query than command (no WHERE clause is present in the former). Based on these 2 commands(Command and ServerCommand), parameter UI can be populated and parameterized queries can be constructed
```csharp
[Obsolete("Use ExternalConnection.SecondCommand property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string SeverCommand { get; set; }
```
### Remarks
NOTE: This property is now obsolete. Instead, please use ExternalConnection.SecondCommand property. This method will be removed 12 months later since October 2024. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
namespace AsposeCellsExamples
{
public class DBConnectionPropertySeverCommandDemo
{
public static void Run()
{
Workbook workbook = new Workbook("input.xlsx");
ExternalConnectionCollection connections = workbook.DataConnections;
foreach (ExternalConnection connection in connections)
{
if (connection is DBConnection dbConn)
{
dbConn.Name = dbConn.Name.Replace("c:\\", "d:\\");
dbConn.SourceFile = dbConn.SourceFile.Replace("c:\\", "d:\\");
dbConn.ConnectionInfo = dbConn.ConnectionInfo.Replace("c:\\", "d:\\").Replace("C:\\", "d:\\");
dbConn.Command = dbConn.Command.Replace("c:\\", "d:\\");
if (!string.IsNullOrEmpty(dbConn.SeverCommand))
dbConn.SeverCommand = dbConn.SeverCommand.Replace("c:\\", "d:\\");
}
}
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)
