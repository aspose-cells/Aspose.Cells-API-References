---
title: ExternalConnection.ConnectionFile
second_title: Aspose.Cells for .NET API Reference
description: ExternalConnection property. Gets the connection file
type: docs
url: /net/aspose.cells.externalconnections/externalconnection/connectionfile/
---
## ExternalConnection.ConnectionFile property

Gets the connection file.

```csharp
public virtual string ConnectionFile { get; }
```

### Examples

```csharp
// Called: Assert.IsNull(conn.ConnectionFile);
[Test]
        public void Property_ConnectionFile()
        {
            Workbook  workbook = new Workbook(Constants.PivotTableSourcePath + &quot;CELLSNET-43799.xlsx&quot;);
            ExternalConnection conn = workbook.Worksheets[0].PivotTables[0].GetSourceDataConnections()[0];
            Assert.AreEqual(&quot;Table1&quot;, conn.Command);
            Assert.IsNull(conn.ConnectionFile);
            workbook.Save(Constants.PivotTableDestPath + &quot;Net43799.xlsx&quot;);
            workbook = new Workbook(Constants.PivotTableDestPath + &quot;Net43799.xlsx&quot;);
            Assert.AreEqual(1, workbook.Worksheets[0].Slicers.Count);
        }
```

### See Also

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


