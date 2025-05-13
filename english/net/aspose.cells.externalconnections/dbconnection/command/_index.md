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
public void DBConnection_Property_Command()
{
    string filePath = Constants.PivotTableSourcePath + @"NET51761_";
    string savePath = CreateFolder(filePath);

    Workbook workbook = new Workbook(filePath + "DataConnectionDetailsGotDeleted.xls");

    DBConnection conn = (DBConnection)workbook.DataConnections[0];

    string command = conn.Command;
    string connectionInfo = conn.ConnectionInfo;
    Console.WriteLine(command);
    Console.WriteLine(connectionInfo);
    Assert.Greater(command.Length, 5);
    Assert.Greater(connectionInfo.Length, 20);
    workbook.Save(savePath + "out.xlsx", Aspose.Cells.SaveFormat.Xlsx);
    workbook.Save(savePath + "out.xlsm", Aspose.Cells.SaveFormat.Xlsm);

    string cacheXml = GetEntryText(savePath + "out.xlsx", @"xl/pivotCache/pivotCacheDefinition1.xml");
    Assert.AreNotEqual(cacheXml.IndexOf("type=\"external\""), -1);

    Workbook wb = new Workbook(savePath + "out.xlsx");
    conn = (DBConnection)wb.DataConnections[0];
    Assert.AreEqual(conn.Command, command);
    Assert.AreEqual(conn.ConnectionInfo, connectionInfo);

}
```

### See Also

* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


