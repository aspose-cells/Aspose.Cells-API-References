---
title: Enum ConnectionDataSourceType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.ExternalConnections.ConnectionDataSourceType enum. Specifies external database source type
type: docs
url: /net/aspose.cells.externalconnections/connectiondatasourcetype/
---
## ConnectionDataSourceType enumeration

Specifies external database source type

```csharp
public enum ConnectionDataSourceType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| ODBCBasedSource | `1` | ODBC-based source |
| DAOBasedSource | `2` | DAO-based source |
| FileBasedDataBaseSource | `3` | File based database source |
| WebQuery | `4` | Web query |
| OLEDBBasedSource | `5` | OLE DB-based source |
| TextBasedSource | `6` | Text-based source |
| ADORecordSet | `7` | ADO record set |
| DSP | `8` | DSP |
| OLEDBDataModel | `100` | OLE DB data source created by the Spreadsheet Data Model. |
| DataFeedDataModel | `101` | Data feed data source created by the Spreadsheet Data Model. |
| WorksheetDataModel | `102` | Worksheet data source created by the Spreadsheet Data Model. |
| Table | `102` | Worksheet data source created by the Spreadsheet Data Model. |
| TextDataModel | `103` | Text data source created by the Spreadsheet Data Model. |
| Unknown | `255` | Text data source created by the Spreadsheet Data Model. |

### Examples

```csharp
// Called: Assert.AreEqual(ConnectionDataSourceType.OLEDBDataModel, conn.SourceType);
[Test]
        public void Type_ConnectionDataSourceType()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + &quot;CellsNet56651.xlsx&quot;);

            ExternalConnection conn = workbook.Worksheets[0].PivotTables[0].GetSourceDataConnections()[0];
            Assert.AreEqual(&quot;721&quot;, conn.Name);
            Assert.AreEqual(ConnectionDataSourceType.OLEDBDataModel, conn.SourceType);
            Assert.AreEqual(@&quot;\\sqaclient\D-Drive\QA_TEAM_Data\Amit Data\CIMCON&apos;s Data\Accounts\1000 mix files\72.xlsx&quot;,conn.ConnectionFile);
          
            Assert.IsTrue(conn.ConnectionString!= null);
            Assert.AreEqual(OLEDBCommandType.TableCollection, conn.CommandType);
            Assert.AreEqual(&quot;\&quot;Sheet1$\&quot;&quot;, conn.Command);

            conn = workbook.Worksheets[1].PivotTables[0].GetSourceDataConnections()[0];
            Assert.AreEqual(&quot;72&quot;, conn.Name);
            Assert.AreEqual(ConnectionDataSourceType.OLEDBBasedSource, conn.SourceType);
            Assert.AreEqual(@&quot;\\sqaclient\D-Drive\QA_TEAM_Data\Amit Data\Risk File\External Data\excel query.xlsx&quot;, conn.ConnectionFile);
           
            Assert.IsTrue(conn.ConnectionString != null);
            Assert.AreEqual(OLEDBCommandType.TableName, conn.CommandType);
            Assert.AreEqual(&quot;Sheet1$&quot;, conn.Command);

        }
```

### See Also

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


