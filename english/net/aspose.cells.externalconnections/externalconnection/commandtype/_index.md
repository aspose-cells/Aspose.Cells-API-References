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
[Test]
        public void Property_CommandType()
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

* enum [OLEDBCommandType](../../oledbcommandtype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


