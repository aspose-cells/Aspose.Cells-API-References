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
private static Worksheet Method_ClearData(Workbook workbook, string sourceData)
        {
            var pivotSheet = workbook.Worksheets.Add(&quot;Pivot Sheet&quot;);

            var pivotTableIndex = pivotSheet.PivotTables.Add(
                sourceData,
                &quot;A1&quot;,
                &quot;PivotTable1&quot;);
            var pivotTable = pivotSheet.PivotTables[pivotTableIndex];
            pivotTable.ClearData();
            pivotTable.ShowInTabularForm();

            pivotTable.AddFieldToArea(PivotFieldType.Row, &quot;Advertiser&quot;);
            pivotTable.AddFieldToArea(PivotFieldType.Row, &quot;Campaign&quot;);
            pivotTable.AddFieldToArea(PivotFieldType.Data, &quot;SpendUSD&quot;);
            pivotTable.AddFieldToArea(PivotFieldType.Data, &quot;Impressions&quot;);

            // Without this, our data fields will be stacked in single column instead of spread across columns.
            //    (http://www.aspose.com/community/forums/thread/316359/creating-pivot-table-with-values-column.aspx)
            pivotTable.AddFieldToArea(PivotFieldType.Column, pivotTable.DataField);

            //pivotTable.ShowValuesRow = false;
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            pivotTable.RefreshDataOnOpeningFile = false;

            var cell = pivotTable.GetCellByDisplayName(&quot;Advertiser&quot;);
            Assert.AreEqual(cell.Name, &quot;A2&quot;);

            pivotTable.ShowValuesRow = false;
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            pivotTable.RefreshDataOnOpeningFile = false;

            cell = pivotTable.GetCellByDisplayName(&quot;Advertiser&quot;);
            workbook.Save(Constants.PivotTableDestPath + @&quot;NET44044.xlsx&quot;);
            Assert.AreEqual(cell.Name, &quot;A1&quot;);

            // However, moving DataField to Column above, we added a &quot;Data&quot; row that&apos;s turned off with the &quot;Show the Values row&quot; option in Excel, so try that here.
            // Unfortunately, it doesn&apos;t seem to matter where this line goes -- it never changes the option on the pivot table.
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


