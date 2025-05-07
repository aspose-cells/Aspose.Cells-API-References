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
// Called: Assert.AreEqual("Table1", conn.Command);
[Test]
        public void Property_Command()
        {
            Workbook  workbook = new Workbook(Constants.PivotTableSourcePath + "CELLSNET-43799.xlsx");
            ExternalConnection conn = workbook.Worksheets[0].PivotTables[0].GetSourceDataConnections()[0];
            Assert.AreEqual("Table1", conn.Command);
            Assert.IsNull(conn.ConnectionFile);
            workbook.Save(Constants.PivotTableDestPath + "Net43799.xlsx");
            workbook = new Workbook(Constants.PivotTableDestPath + "Net43799.xlsx");
            Assert.AreEqual(1, workbook.Worksheets[0].Slicers.Count);
        }
```

### See Also

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


