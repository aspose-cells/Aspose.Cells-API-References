---
title: Enum ExternalConnectionClassType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.ExternalConnections.ExternalConnectionClassType enum. Represents the type of connection
type: docs
url: /net/aspose.cells.externalconnections/externalconnectionclasstype/
---
## ExternalConnectionClassType enumeration

Represents the type of connection

```csharp
public enum ExternalConnectionClassType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Database | `0` | ODBC or OLE DB |
| WebQuery | `1` | Web query |
| TextBased | `2` | Based on text |
| DataModel | `3` | Data model |
| Unkown | `4` |  |

### Examples

```csharp
// Called: Assert.AreEqual(ExternalConnectionClassType.DataModel, conn.ClassType);
[Test]
        public void Type_ExternalConnectionClassType()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + &quot;CELLSNET56781.xlsx&quot;);

            ExternalConnection conn = workbook.Worksheets[0].PivotTables[0].GetSourceDataConnections()[0];
            Assert.AreEqual(&quot;WorksheetConnection_Sheet3!$B$2:$C$114&quot;, conn.Name);
            Assert.AreEqual(ExternalConnectionClassType.DataModel, conn.ClassType);
           Assert.AreEqual(ConnectionDataSourceType.WorksheetDataModel, conn.SourceType);
           Assert.IsNull(conn.ConnectionFile);
            Assert.IsNull(conn.ConnectionString);

            Assert.AreEqual(&quot;Sheet3!$B$2:$C$114&quot;, conn.Command);


            conn = workbook.Worksheets[1].PivotTables[0].GetSourceDataConnections()[0];
            Assert.AreEqual(&quot;Data3&quot;,conn.Command);
            workbook.Save(Constants.PivotTableDestPath + &quot;CELLSNET56781.xlsx&quot;);
        }
```

### See Also

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


