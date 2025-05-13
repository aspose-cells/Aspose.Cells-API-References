---
title: ExternalConnection.ConnectionFile
second_title: Aspose.Cells for .NET API Reference
description: ExternalConnection property. Gets the connection file
type: docs
url: /net/aspose.cells.externalconnections/externalconnection/connectionfile/
---
## ExternalConnection.ConnectionFile property

Gets the connection file.

```csharp
public virtual string ConnectionFile { get; }
```

### Examples

```csharp
// Called: Assert.IsNull(conn.ConnectionFile);
public void ExternalConnection_Property_ConnectionFile()
{
    Workbook  workbook = new Workbook(Constants.PivotTableSourcePath + "example.xlsx");
    ExternalConnection conn = workbook.Worksheets[0].PivotTables[0].GetSourceDataConnections()[0];
    Assert.AreEqual("Table1", conn.Command);
    Assert.IsNull(conn.ConnectionFile);
    workbook.Save(Constants.PivotTableDestPath + "example.xlsx");
    workbook = new Workbook(Constants.PivotTableDestPath + "example.xlsx");
    Assert.AreEqual(1, workbook.Worksheets[0].Slicers.Count);
}
```

### See Also

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


