---
title: PivotTable.GetSourceDataConnections
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Gets the external connection data sources
type: docs
url: /net/aspose.cells.pivot/pivottable/getsourcedataconnections/
---
## PivotTable.GetSourceDataConnections method

Gets the external connection data sources.

```csharp
public ExternalConnection[] GetSourceDataConnections()
```

### Examples

```csharp
// Called: Assert.IsTrue(wb.Worksheets[0].PivotTables[0].GetSourceDataConnections()[0].ConnectionString != null);
[Test]
        public void Method_GetSourceDataConnections()
        {
            Workbook wb = new Workbook(Constants.PivotTableSourcePath + "CELLSNET57862.xlsx");
            // wb.Worksheets[0].PivotTables.Clear();
            wb.Save(Constants.PivotTableDestPath + "CELLSNET57862.xls");
            wb = new Workbook(Constants.PivotTableDestPath + "CELLSNET57862.xls");
            wb.Save(Constants.PivotTableDestPath + "CELLSNET57862.xlsx");
            Assert.IsTrue(wb.Worksheets[0].PivotTables[0].GetSourceDataConnections()[0].ConnectionString != null);
            Assert.AreEqual("RegressionTestingForClients TestingTime$",wb.Worksheets[0].PivotTables[0].GetSourceDataConnections()[0].Name);
        }
```

### See Also

* class [ExternalConnection](../../../aspose.cells.externalconnections/externalconnection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


