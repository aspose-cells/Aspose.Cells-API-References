---
title: Workbook.DataConnections
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Gets the ExternalConnection collection
type: docs
url: /net/aspose.cells/workbook/dataconnections/
---
## Workbook.DataConnections property

Gets the [`ExternalConnection`](../../../aspose.cells.externalconnections/externalconnection/) collection.

```csharp
public ExternalConnectionCollection DataConnections { get; }
```

### Examples

```csharp
// Called: Aspose.Cells.ExternalConnections.DBConnection conn = (Aspose.Cells.ExternalConnections.DBConnection)workbook.DataConnections[1];
[Test]
        public void Property_DataConnections()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet51772.xls");
            Aspose.Cells.ExternalConnections.DBConnection conn = (Aspose.Cells.ExternalConnections.DBConnection)workbook.DataConnections[1];
            Assert.IsTrue(conn.ConnectionInfo.StartsWith("Provider=MSOLAP.4;Integrated Security=SSPI;"));
            workbook.Save(Constants.destPath + "CellsNet51772.xlsx");
            workbook = new Workbook(Constants.destPath + "CellsNet51772.xlsx");
            conn = (Aspose.Cells.ExternalConnections.DBConnection)workbook.DataConnections[1];
            Assert.IsTrue(conn.ConnectionInfo.StartsWith("Provider=MSOLAP.4;Integrated Security=SSPI;"));
            Assert.AreEqual(0, workbook.Worksheets[0].PivotTables.Count);//CELLSNET-56866
        }
```

### See Also

* class [ExternalConnectionCollection](../../../aspose.cells.externalconnections/externalconnectioncollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


