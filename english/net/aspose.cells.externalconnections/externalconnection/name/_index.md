---
title: ExternalConnection.Name
second_title: Aspose.Cells for .NET API Reference
description: ExternalConnection property. Specifies the name of the connection. Each connection must have a unique name
type: docs
url: /net/aspose.cells.externalconnections/externalconnection/name/
---
## ExternalConnection.Name property

Specifies the name of the connection. Each connection must have a unique name.

```csharp
public string Name { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual("WorksheetConnection_pivot.xlsx!テーブル3", conns[0].Name);
[Test]
        public void Property_Name()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "CELLSPYTHONNET190.xlsx");
            ExternalConnection[] conns = workbook.Worksheets[0].PivotTables[0].GetSourceDataConnections();
            Assert.AreEqual("WorksheetConnection_pivot.xlsx!テーブル3", conns[0].Name);
            Assert.AreEqual("テーブル3", conns[0].Command);
            workbook.Save(Constants.PivotTableDestPath + "CELLSPYTHONNET190_1.xlsx");
        }
```

### See Also

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


