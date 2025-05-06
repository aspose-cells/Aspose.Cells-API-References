---
title: PivotTable.GetNamesOfSourceDataConnections
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Gets the name of external source data connections
type: docs
url: /net/aspose.cells.pivot/pivottable/getnamesofsourcedataconnections/
---
## PivotTable.GetNamesOfSourceDataConnections method

Gets the name of external source data connections.

```csharp
public string[] GetNamesOfSourceDataConnections()
```

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;WorksheetConnection_PivotTableReferences.xlsx!Data3&amp;quot;, pt.GetNamesOfSourceDataConnections()[0]);
[Test]
        public void Method_GetNamesOfSourceDataConnections()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + &quot;CELLSNET56780.xlsx&quot;);
            PivotTable pt = workbook.Worksheets[0].PivotTables[0];
            Assert.AreEqual(&quot;WorksheetConnection_Sheet3!$B$2:$C$114&quot;, pt.GetNamesOfSourceDataConnections()[0]);
            Assert.IsTrue(pt.GetNamesOfSourceDataConnections()[0] != null);

            pt = workbook.Worksheets[1].PivotTables[0];
            Assert.AreEqual(&quot;WorksheetConnection_PivotTableReferences.xlsx!Data3&quot;, pt.GetNamesOfSourceDataConnections()[0]);
            Assert.IsTrue(pt.GetNamesOfSourceDataConnections()[0] != null);
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


