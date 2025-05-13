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
// Called: Assert.AreEqual("WorksheetConnection_Sheet3!$B$2:$C$114", pt.GetNamesOfSourceDataConnections()[0]);
public void PivotTable_Method_GetNamesOfSourceDataConnections()
{
    Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "example.xlsx");
    PivotTable pt = workbook.Worksheets[0].PivotTables[0];
    Assert.AreEqual("WorksheetConnection_Sheet3!$B$2:$C$114", pt.GetNamesOfSourceDataConnections()[0]);
    Assert.IsTrue(pt.GetNamesOfSourceDataConnections()[0] != null);

    pt = workbook.Worksheets[1].PivotTables[0];
    Assert.AreEqual("WorksheetConnection_PivotTableReferences.xlsx!Data3", pt.GetNamesOfSourceDataConnections()[0]);
    Assert.IsTrue(pt.GetNamesOfSourceDataConnections()[0] != null);
}
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


