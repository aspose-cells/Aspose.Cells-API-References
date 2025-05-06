---
title: Cells.FirstCell
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Gets the first cell in this worksheet
type: docs
url: /net/aspose.cells/cells/firstcell/
---
## Cells.FirstCell property

Gets the first cell in this worksheet.

```csharp
public Cell FirstCell { get; }
```

### Remarks

Returns null if there is no data in the worksheet.

### Examples

```csharp
// Called: int pivotIndex = pivotTableCollection.Add(&amp;quot;Data1!&amp;quot; + wsData.Cells.FirstCell.Name + &amp;quot;:&amp;quot; + wsData.Cells.LastCell.Name, &amp;quot;A1&amp;quot;, &amp;quot;Pivot12&amp;quot;);
[Test]
        public void Property_FirstCell()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET46572_&quot;;

            //Open the source file
            Workbook wb11 = new Workbook(filePath + @&quot;xlsbdatasource1.xlsx&quot;);
            DataTable dtGetExcelData = wb11.Worksheets[0].Cells.ExportDataTable(0, 0, wb11.Worksheets[0].Cells.MaxRow + 1, wb11.Worksheets[0].Cells.MaxColumn + 1);
            //add the data sheet
            Workbook wbAct = new Workbook();
            var wsData = wbAct.Worksheets[wbAct.Worksheets.Add()];
            wsData.Name = &quot;Data1&quot;;
            //import data
            wsData.Cells.ImportData(dtGetExcelData, 0, 0, new ImportTableOptions() { IsFieldNameShown = true });

            //Add Pivot sheet
            var ws = wbAct.Worksheets[wbAct.Worksheets.Add()];
            ws.Name = &quot;Pvt_Detailed_Sht&quot;;

            var pivotTableCollection = ws.PivotTables;
            int pivotIndex = pivotTableCollection.Add(&quot;Data1!&quot; + wsData.Cells.FirstCell.Name + &quot;:&quot; + wsData.Cells.LastCell.Name, &quot;A1&quot;, &quot;Pivot12&quot;);
            var pivotTable = pivotTableCollection[pivotIndex];

            pivotTable.ShowRowGrandTotals = true;
            pivotTable.ShowColumnGrandTotals = true;

            //Add row fields
            var idx = pivotTable.AddFieldToArea(PivotFieldType.Row, 1);
            pivotTable.RowFields[idx].IsAutoSubtotals = false;
            pivotTable.RowFields[idx].IsRepeatItemLabels = true;

            var idx1 = pivotTable.AddFieldToArea(PivotFieldType.Row, 7);
            pivotTable.RowFields[idx1].IsAutoSubtotals = false;
            pivotTable.RowFields[idx1].IsRepeatItemLabels = true;

            // When more than 1 data field is added xlsb file gets corrupted. If only 1 data column is added xlsb file is not corrupted
            // Xlsx is not corrupted even when multiple data fields are added.
            // add only 1 data column both xlsx and xlsb works fine

            pivotTable.AddFieldToArea(PivotFieldType.Data, &quot;Column31&quot;);
            pivotTable.AddFieldToArea(PivotFieldType.Data, &quot;Column32&quot;);

            pivotTable.RefreshData();
            pivotTable.CalculateData();

            wbAct.Worksheets.RemoveAt(0);

            wbAct.Save(Constants.PIVOT_CHECK_FILE_PATH + @&quot;NET46572_Corrupted-Datacolsmorethan1.Xlsb&quot;, SaveFormat.Xlsb);
            //xlsx file coming uncorrupted.
            wbAct.Save(Constants.PIVOT_CHECK_FILE_PATH + @&quot;NET46572_Datacolsmorethan1.Xlsx&quot;, SaveFormat.Xlsx);
        }
```

### See Also

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


