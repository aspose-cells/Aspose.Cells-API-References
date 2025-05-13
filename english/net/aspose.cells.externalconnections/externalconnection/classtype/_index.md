---
title: ExternalConnection.ClassType
second_title: Aspose.Cells for .NET API Reference
description: ExternalConnection property. Gets the type of this ExternalConnection object
type: docs
url: /net/aspose.cells.externalconnections/externalconnection/classtype/
---
## ExternalConnection.ClassType property

Gets the type of this [`ExternalConnection`](../) object.

```csharp
public abstract ExternalConnectionClassType ClassType { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(ExternalConnectionClassType.DataModel, conn.ClassType);
public void ExternalConnection_Property_ClassType()
{
    Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "example.xlsx");

    ExternalConnection conn = workbook.Worksheets[0].PivotTables[0].GetSourceDataConnections()[0];
    Assert.AreEqual("WorksheetConnection_Sheet3!$B$2:$C$114", conn.Name);
    Assert.AreEqual(ExternalConnectionClassType.DataModel, conn.ClassType);
   Assert.AreEqual(ConnectionDataSourceType.WorksheetDataModel, conn.SourceType);
   Assert.IsNull(conn.ConnectionFile);
    Assert.IsNull(conn.ConnectionString);

    Assert.AreEqual("Sheet3!$B$2:$C$114", conn.Command);


    conn = workbook.Worksheets[1].PivotTables[0].GetSourceDataConnections()[0];
    Assert.AreEqual("Data3",conn.Command);
    workbook.Save(Constants.PivotTableDestPath + "example.xlsx");
}
```

### See Also

* enum [ExternalConnectionClassType](../../externalconnectionclasstype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


