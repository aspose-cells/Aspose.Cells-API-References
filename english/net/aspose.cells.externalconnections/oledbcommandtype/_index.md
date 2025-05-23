---
title: Enum OLEDBCommandType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.ExternalConnections.OLEDBCommandType enum. Specifies the OLE DB command type
type: docs
url: /net/aspose.cells.externalconnections/oledbcommandtype/
---
## OLEDBCommandType enumeration

Specifies the OLE DB command type.

```csharp
public enum OLEDBCommandType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| None | `0` | The command type is not specified. |
| CubeName | `1` | Specifies a cube name |
| SqlStatement | `2` | Specifies a SQL statement |
| TableName | `3` | Specifies a table name |
| DefaultInformation | `4` | Specifies that default information has been given, and it is up to the provider how to interpret. |
| WebBasedList | `5` | Specifies a query which is against a web based List Data Provider. |
| TableCollection | `6` | Specifies the table list. |

### Examples

```csharp
// Called: Assert.AreEqual(OLEDBCommandType.TableName, conn.CommandType);
public void ExternalConnections_Type_OLEDBCommandType()
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

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


