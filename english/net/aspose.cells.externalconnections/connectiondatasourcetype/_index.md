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
// Called: Assert.AreEqual(ConnectionDataSourceType.WorksheetDataModel, conn.SourceType);
[Test]
        public void Type_ConnectionDataSourceType()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "CELLSNET56781.xlsx");

            ExternalConnection conn = workbook.Worksheets[0].PivotTables[0].GetSourceDataConnections()[0];
            Assert.AreEqual("WorksheetConnection_Sheet3!$B$2:$C$114", conn.Name);
            Assert.AreEqual(ExternalConnectionClassType.DataModel, conn.ClassType);
           Assert.AreEqual(ConnectionDataSourceType.WorksheetDataModel, conn.SourceType);
           Assert.IsNull(conn.ConnectionFile);
            Assert.IsNull(conn.ConnectionString);

            Assert.AreEqual("Sheet3!$B$2:$C$114", conn.Command);


            conn = workbook.Worksheets[1].PivotTables[0].GetSourceDataConnections()[0];
            Assert.AreEqual("Data3",conn.Command);
            workbook.Save(Constants.PivotTableDestPath + "CELLSNET56781.xlsx");
        }
```

### See Also

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


