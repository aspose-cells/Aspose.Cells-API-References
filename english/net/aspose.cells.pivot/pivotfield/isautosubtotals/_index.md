---
title: PivotField.IsAutoSubtotals
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Indicates whether the specified field shows automatic subtotals. Default is true
type: docs
url: /net/aspose.cells.pivot/pivotfield/isautosubtotals/
---
## PivotField.IsAutoSubtotals property

Indicates whether the specified field shows automatic subtotals. Default is true.

```csharp
public bool IsAutoSubtotals { get; set; }
```

### Examples

```csharp
// Called: pivotTable.RowFields[idx].IsAutoSubtotals = false;
[Test]
        public void Property_IsAutoSubtotals()
        {
            string filePath = Constants.PivotTableSourcePath + @&quot;NET46678_&quot;;

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

            string savePath = CreateFolder(filePath);
            wbAct.Save(savePath + @&quot;out.Xlsb&quot;, SaveFormat.Xlsb);
            //xlsx file coming uncorrupted.
            wbAct.Save(savePath + @&quot;out.Xlsx&quot;, SaveFormat.Xlsx);

            wbAct = new Workbook(savePath + &quot;out.Xlsb&quot;);
            Assert.AreEqual(wbAct.Worksheets[1].PivotTables[0].RowFields[0].IsRepeatItemLabels, true);
            Assert.AreEqual(wbAct.Worksheets[1].PivotTables[0].RowFields[1].IsRepeatItemLabels, true);
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


