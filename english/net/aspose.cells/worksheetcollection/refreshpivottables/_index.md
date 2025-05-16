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

### Examples

```csharp
namespace AsposeCellsExamples.WorksheetCollectionMethodRefreshPivotTablesWithPivotTableRefreshOptionDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class WorksheetCollectionMethodRefreshPivotTablesWithPivotTableRefreshOptionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            cells["A1"].Value = "Category";
            cells["A2"].Value = "Fruit";
            cells["A3"].Value = "Vegetable";
            cells["B1"].Value = "Sales";
            cells["B2"].Value = 1500;
            cells["B3"].Value = 2300;

            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B3", "E5", "SalesPivot");
            PivotTable pivotTable = pivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            pivotTable.RefreshData();

            cells["B2"].Value = 2000;

            PivotTableRefreshOption option = new PivotTableRefreshOption();

            try
            {
                bool success = workbook.Worksheets.RefreshPivotTables(option);
                Console.WriteLine($"Pivot tables refreshed: {success}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error refreshing pivot tables: {ex.Message}");
            }

            workbook.Save("WorksheetCollectionMethodRefreshPivotTablesWithPivotTableRefreshOptionDemo.xlsx");
        }
    }
}
```

### See Also

* class [PivotTableRefreshOption](../../../aspose.cells.pivot/pivottablerefreshoption/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


