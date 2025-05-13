---
title: PivotTable.ClearData
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Clear PivotTables data and formatting
type: docs
url: /net/aspose.cells.pivot/pivottable/cleardata/
---
## PivotTable.ClearData method

Clear PivotTable's data and formatting

```csharp
public void ClearData()
```

### Remarks

If this method is not called before you add or delete PivotField, Maybe the PivotTable data is not corrected

### Examples

```csharp
// Called: pivotTable.ClearData();
private static Worksheet PivotTable_Method_ClearData(Workbook workbook, string sourceData)
        {
            var pivotSheet = workbook.Worksheets.Add("Pivot Sheet");

            var pivotTableIndex = pivotSheet.PivotTables.Add(
                sourceData,
                "A1",
                "PivotTable1");
            var pivotTable = pivotSheet.PivotTables[pivotTableIndex];
            pivotTable.ClearData();
            pivotTable.ShowInTabularForm();

            pivotTable.AddFieldToArea(PivotFieldType.Row, "Advertiser");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Campaign");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "SpendUSD");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Impressions");

            // Without this, our data fields will be stacked in single column instead of spread across columns.
            //    (http://www.aspose.com/community/forums/thread/316359/creating-pivot-table-with-values-column.aspx)
            pivotTable.AddFieldToArea(PivotFieldType.Column, pivotTable.DataField);

            //pivotTable.ShowValuesRow = false;
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            pivotTable.RefreshDataOnOpeningFile = false;

            var cell = pivotTable.GetCellByDisplayName("Advertiser");
            Assert.AreEqual(cell.Name, "A2");

            pivotTable.ShowValuesRow = false;
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            pivotTable.RefreshDataOnOpeningFile = false;

            cell = pivotTable.GetCellByDisplayName("Advertiser");
            workbook.Save(Constants.PivotTableDestPath + @"example.xlsx");
            Assert.AreEqual(cell.Name, "A1");

            // However, moving DataField to Column above, we added a "Data" row that's turned off with the "Show the Values row" option in Excel, so try that here.
            // Unfortunately, it doesn't seem to matter where this line goes -- it never changes the option on the pivot table.
            //

            // PROBLEM: THIS NEXT LINE HAS NO EFFECT
            //pivotTable.ShowValuesRow = false;

            return pivotSheet;
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


