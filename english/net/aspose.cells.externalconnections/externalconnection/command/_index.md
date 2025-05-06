---
title: ExternalConnection.Command
second_title: Aspose.Cells for .NET API Reference
description: ExternalConnection property. The string containing the database command to pass to the data provider API that will interact with the external source in order to retrieve data
type: docs
url: /net/aspose.cells.externalconnections/externalconnection/command/
---
## ExternalConnection.Command property

The string containing the database command to pass to the data provider API that will interact with the external source in order to retrieve data

```csharp
public virtual string Command { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;テーブル3&amp;quot;, conns[0].Command);
[Test]
        public void Property_Command()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + &quot;CELLSPYTHONNET190.xlsx&quot;);
            ExternalConnection[] conns = workbook.Worksheets[0].PivotTables[0].GetSourceDataConnections();
            Assert.AreEqual(&quot;WorksheetConnection_pivot.xlsx!テーブル3&quot;, conns[0].Name);
            Assert.AreEqual(&quot;テーブル3&quot;, conns[0].Command);
            workbook.Save(Constants.PivotTableDestPath + &quot;CELLSPYTHONNET190_1.xlsx&quot;);
        }
```

### See Also

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


