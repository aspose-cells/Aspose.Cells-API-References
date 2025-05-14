---
title: ExternalConnection.CommandType
second_title: Aspose.Cells for .NET API Reference
description: ExternalConnection property. Specifies the OLE DB command type. 1. Query specifies a cube name 2. Query specifies a SQL statement 3. Query specifies a table name 4. Query specifies that default information has been given and it is up to the provider how to interpret. 5. Query is against a web based List Data Provider
type: docs
url: /net/aspose.cells.externalconnections/externalconnection/commandtype/
---
## ExternalConnection.CommandType property

Specifies the OLE DB command type. 1. Query specifies a cube name 2. Query specifies a SQL statement 3. Query specifies a table name 4. Query specifies that default information has been given, and it is up to the provider how to interpret. 5. Query is against a web based List Data Provider.

```csharp
public virtual OLEDBCommandType CommandType { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(OLEDBCommandType.TableCollection, conn.CommandType);
public void ExternalConnection_Property_CommandType()
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

* enum [OLEDBCommandType](../../oledbcommandtype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


