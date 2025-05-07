---
title: PivotTable.DataField
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Gets a PivotField object that represents all the data fields in a PivotTable. Readonly. It would only be created when there are two or more data fields in the Data region. Defaultly it is in row region. You can drag it to the row/column region with PivotTable.AddFieldToArea method 
type: docs
url: /net/aspose.cells.pivot/pivottable/datafield/
---
## PivotTable.DataField property

Gets a [`PivotField`](../../pivotfield/) object that represents all the data fields in a PivotTable. Read-only. It would only be created when there are two or more data fields in the Data region. Defaultly it is in row region. You can drag it to the row/column region with PivotTable.AddFieldToArea() method .

```csharp
public PivotField DataField { get; }
```

### Examples

```csharp
// Called: pivotTable.AddFieldToArea(PivotFieldType.Column, pivotTable.DataField);
private static Worksheet Property_DataField(Workbook workbook, string sourceData)
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
            workbook.Save(Constants.PivotTableDestPath + @"NET44044.xlsx");
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

* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


