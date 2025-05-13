---
title: DBConnection.ConnectionInfo
second_title: Aspose.Cells for .NET API Reference
description: DBConnection property. The connection information string is used to make contact with an OLE DB or ODBC data source
type: docs
url: /net/aspose.cells.externalconnections/dbconnection/connectioninfo/
---
## DBConnection.ConnectionInfo property

The connection information string is used to make contact with an OLE DB or ODBC data source.

```csharp
[Obsolete("Use ExternalConnection.ConnectionString property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string ConnectionInfo { get; set; }
```

### Remarks

NOTE: This property is now obsolete. Instead, please use ExternalConnection.ConnectionString property. This method will be removed 12 months later since October 2024. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: if (string.IsNullOrEmpty(c.ConnectionInfo))
public void DBConnection_Property_ConnectionInfo()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    ExternalConnectionCollection conns = workbook.DataConnections;
    DBConnection c = (DBConnection)conns[4];
    if (string.IsNullOrEmpty(c.ConnectionInfo))
    {
        Assert.Fail("DBConnection.ConnectionInfo should not be empty or null");
    }
}
```

### See Also

* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


