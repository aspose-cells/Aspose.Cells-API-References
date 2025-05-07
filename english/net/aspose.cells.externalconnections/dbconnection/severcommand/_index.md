---
title: DBConnection.SeverCommand
second_title: Aspose.Cells for .NET API Reference
description: DBConnection property. Specifies a second command text string that is persisted when PivotTable serverbased page fields are in use. For ODBC connections serverCommand is usually a broader query than command no WHERE clause is present in the former. Based on these 2 commandsCommand and ServerCommand parameter UI can be populated and parameterized queries can be constructed
type: docs
url: /net/aspose.cells.externalconnections/dbconnection/severcommand/
---
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
// Called: connection.SeverCommand = connection.SeverCommand.Replace("c:\\", "d:\\");
[Test]
        public void Property_SeverCommand()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET46959.xls");
            Aspose.Cells.ExternalConnections.ExternalConnectionCollection connections = workbook.DataConnections;

            foreach (Aspose.Cells.ExternalConnections.DBConnection connection in connections)
            {
                connection.Name = connection.Name.Replace("c:\\", "d:\\");
                connection.SourceFile = connection.SourceFile.Replace("c:\\", "d:\\");
                connection.ConnectionInfo = connection.ConnectionInfo.Replace("c:\\", "d:\\").Replace("C:\\", "d:\\");
                connection.Command = connection.Command.Replace("c:\\", "d:\\");
                if (!string.IsNullOrEmpty(connection.SeverCommand))
                    connection.SeverCommand = connection.SeverCommand.Replace("c:\\", "d:\\");
            }
            workbook.Save(Constants.destPath + "CELLSNET46959.xls");
        }
```

### See Also

* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


