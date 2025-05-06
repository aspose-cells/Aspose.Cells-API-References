---
title: DBConnection.Command
second_title: Aspose.Cells for .NET API Reference
description: DBConnection property. The string containing the database command to pass to the data provider API that will interact with the external source in order to retrieve data
type: docs
url: /net/aspose.cells.externalconnections/dbconnection/command/
---
## DBConnection.Command property

The string containing the database command to pass to the data provider API that will interact with the external source in order to retrieve data

```csharp
public override string Command { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(conn.Command, command);
[Test]
        public void Property_Command()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET51761_&quot;;
            string savePath = CreateFolder(filePath);

            Workbook workbook = new Workbook(filePath + &quot;DataConnectionDetailsGotDeleted.xls&quot;);

            DBConnection conn = (DBConnection)workbook.DataConnections[0];

            string command = conn.Command;
            string connectionInfo = conn.ConnectionInfo;
            Console.WriteLine(command);
            Console.WriteLine(connectionInfo);
            Assert.Greater(command.Length, 5);
            Assert.Greater(connectionInfo.Length, 20);
            workbook.Save(savePath + &quot;out.xlsx&quot;, Aspose.Cells.SaveFormat.Xlsx);
            workbook.Save(savePath + &quot;out.xlsm&quot;, Aspose.Cells.SaveFormat.Xlsm);

            string cacheXml = GetEntryText(savePath + &quot;out.xlsx&quot;, @&quot;xl/pivotCache/pivotCacheDefinition1.xml&quot;);
            Assert.AreNotEqual(cacheXml.IndexOf(&quot;type=\&quot;external\&quot;&quot;), -1);

            Workbook wb = new Workbook(savePath + &quot;out.xlsx&quot;);
            conn = (DBConnection)wb.DataConnections[0];
            Assert.AreEqual(conn.Command, command);
            Assert.AreEqual(conn.ConnectionInfo, connectionInfo);

        }
```

### See Also

* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


