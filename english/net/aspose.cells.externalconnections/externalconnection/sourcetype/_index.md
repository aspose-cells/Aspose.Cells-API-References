---
title: ExternalConnection.SourceType
second_title: Aspose.Cells for .NET API Reference
description: ExternalConnection property. Gets or Sets the external connection DataSource type
type: docs
url: /net/aspose.cells.externalconnections/externalconnection/sourcetype/
---
## ExternalConnection.SourceType property

Gets or Sets the external connection DataSource type.

```csharp
public ConnectionDataSourceType SourceType { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(ConnectionDataSourceType.OLEDBDataModel, conn.SourceType);
public void ExternalConnection_Property_SourceType()
{
    Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "example.xlsx");

    ExternalConnection conn = workbook.Worksheets[0].PivotTables[0].GetSourceDataConnections()[0];
    Assert.AreEqual("721", conn.Name);
    Assert.AreEqual(ConnectionDataSourceType.OLEDBDataModel, conn.SourceType);
    Assert.AreEqual(@"\\sqaclient\D-Drive\QA_TEAM_Data\Amit Data\CIMCON'example.xlsx',conn.ConnectionFile);
          
    Assert.IsTrue(conn.ConnectionString!= null);
    Assert.AreEqual(OLEDBCommandType.TableCollection, conn.CommandType);
    Assert.AreEqual("\"Sheet1$\"", conn.Command);

    conn = workbook.Worksheets[1].PivotTables[0].GetSourceDataConnections()[0];
    Assert.AreEqual("72", conn.Name);
    Assert.AreEqual(ConnectionDataSourceType.OLEDBBasedSource, conn.SourceType);
    Assert.AreEqual(@"\\sqaclient\D-Drive\QA_TEAM_Data\Amit Data\Risk File\External Data\excel query.xlsx", conn.ConnectionFile);
           
    Assert.IsTrue(conn.ConnectionString != null);
    Assert.AreEqual(OLEDBCommandType.TableName, conn.CommandType);
    Assert.AreEqual("Sheet1$", conn.Command);

}
```

### See Also

* enum [ConnectionDataSourceType](../../connectiondatasourcetype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


