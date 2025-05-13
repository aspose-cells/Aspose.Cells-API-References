---
title: ExternalConnection.SourceFile
second_title: Aspose.Cells for .NET API Reference
description: ExternalConnection property. Used when the external data source is filebased. When a connection to such a data source fails the spreadsheet application attempts to connect directly to this file. May be expressed in URI or systemspecific file path notation
type: docs
url: /net/aspose.cells.externalconnections/externalconnection/sourcefile/
---
## ExternalConnection.SourceFile property

Used when the external data source is file-based. When a connection to such a data source fails, the spreadsheet application attempts to connect directly to this file. May be expressed in URI or system-specific file path notation.

```csharp
public string SourceFile { get; set; }
```

### Examples

```csharp
// Called: connection.SourceFile = connection.SourceFile.Replace("c:\\", "d:\\");
public void ExternalConnection_Property_SourceFile()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
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
    workbook.Save(Constants.destPath + "example.xls");
}
```

### See Also

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


