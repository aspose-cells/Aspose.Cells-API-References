---
title: WorksheetCollection.RefreshPivotTables
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection method. Refreshes all the PivotTables in the Excel file
type: docs
url: /net/aspose.cells/worksheetcollection/refreshpivottables/
---
## RefreshPivotTables() {#refreshpivottables_1}

Refreshes all the PivotTables in the Excel file.

```csharp
public void RefreshPivotTables()
```

### Examples

```csharp
// Called: workbook.Worksheets.RefreshPivotTables();
public void WorksheetCollection_Method_RefreshPivotTables()
{
    Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "example.xlsx");
    workbook.Worksheets.RefreshPivotTables();
    Assert.AreEqual("", workbook.Worksheets[0].Cells["B8"].StringValue);
    Assert.AreEqual("", workbook.Worksheets[0].Cells["B9"].StringValue);
}
```

### See Also

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RefreshPivotTables(PivotTableRefreshOption) {#refreshpivottables}

Refreshes all the PivotTables in the Excel file.

```csharp
public bool RefreshPivotTables(PivotTableRefreshOption option)
```

| Parameter | Type | Description |
| --- | --- | --- |
| option | PivotTableRefreshOption | The option for refreshing data source of the pivot tables. |

### See Also

* class [PivotTableRefreshOption](../../../aspose.cells.pivot/pivottablerefreshoption/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


