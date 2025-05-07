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
[Test]
        public void Method_RefreshPivotTables()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "CellsNet55076_1.xlsx");
            workbook.Worksheets.RefreshPivotTables();
            workbook.Save(Constants.PivotTableDestPath + "CellsNet55076_1.xlsx");
#if NET6_0_OR_GREATER
            Assert.AreEqual("5-5.1", workbook.Worksheets[0].Cells["D12"].StringValue);
            Assert.AreEqual("5.9-6", workbook.Worksheets[0].Cells["D11"].StringValue);
#else
            Assert.AreEqual("5-5.1", workbook.Worksheets[0].Cells["D11"].StringValue);
            Assert.AreEqual("5.9-6", workbook.Worksheets[0].Cells["D12"].StringValue);
#endif

            Assert.AreEqual("4-4.1", workbook.Worksheets[0].Cells["D13"].StringValue);
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


