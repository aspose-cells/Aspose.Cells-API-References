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
[Test]
        public void Property_SourceType()
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

* enum [ConnectionDataSourceType](../../connectiondatasourcetype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


