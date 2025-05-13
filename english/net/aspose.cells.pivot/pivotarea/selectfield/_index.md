---
title: PivotArea.SelectField
second_title: Aspose.Cells for .NET API Reference
description: PivotArea method. Select a field in the region as an area
type: docs
url: /net/aspose.cells.pivot/pivotarea/selectfield/
---
## SelectField(PivotFieldType, string) {#selectfield_1}

Select a field in the region as an area.

```csharp
public void SelectField(PivotFieldType axisType, string fieldName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| axisType | PivotFieldType | The region type. |
| fieldName | String | The name of pivot field. |

### Examples

```csharp
// Called: pivotArea.SelectField(PivotFieldType.Row, "CommonName");
public void PivotArea_Method_SelectField()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    PivotTableCollection pivotTables;
    PivotTable pivotTable;
    PivotField pivotField;
    PivotItemCollection pivotItems;
    PivotItem pivotItem;
    PivotFieldCollection pivotDataFields;

    int pivotTableIndex;

    Worksheet detailWorksheet = workbook.Worksheets["Detail"];


    Worksheet worksheet = workbook.Worksheets.Add("RENEWALS WITH LR >= 40%");
    worksheet.TabColor = Color.Red;

    pivotTables = worksheet.PivotTables;

    pivotTableIndex = pivotTables.Add($"'Detail'!A1:{CellsHelper.CellIndexToName(detailWorksheet.Cells.MaxDataRow, detailWorksheet.Cells.MaxDataColumn)}", "A1", "PivotTable1");

    pivotTable = pivotTables[pivotTableIndex];

    pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleLight16;

    pivotTable.ShowValuesRow = false;

    //RowFields
    pivotTable.AddFieldToArea(PivotFieldType.Row, "MonthDay");

    //Uncheck "(blank)" item
    pivotField = pivotTable.RowFields["MonthDay"];
    pivotField.IsAutoSort = true;
    pivotField.IsAscendSort = true;

    pivotItems = pivotField.PivotItems;

    for (int i = 0; i < pivotItems.Count; i++)
    {
        pivotItem = pivotItems[i];
        if (pivotItem.Name != null && pivotItem.Name.Equals("(blank)"))
        {
            pivotItem.IsHidden = true;
        }
    }

    pivotTable.AddFieldToArea(PivotFieldType.Row, "CommonName");

    pivotTable.AddFieldToArea(PivotFieldType.Row, "PolicyNumber");
    pivotField = pivotTable.RowFields["PolicyNumber"];
    //Hide Subtotal
    pivotField.IsAutoSubtotals = false;

    pivotTable.AddFieldToArea(PivotFieldType.Row, "CoveragePart");
    pivotField = pivotTable.RowFields["CoveragePart"];
    //Hide Subtotal
    pivotField.IsAutoSubtotals = false;

    pivotTable.AddFieldToArea(PivotFieldType.Row, "ExpDate");
    pivotField = pivotTable.RowFields["ExpDate"];
    //Hide Subtotal
    pivotField.IsAutoSubtotals = false;

    pivotTable.AddFieldToArea(PivotFieldType.Row, "ClaimCount");

    //DataFields
    pivotTable.AddFieldToArea(PivotFieldType.Data, "Written");
    pivotTable.AddFieldToArea(PivotFieldType.Data, "Earned");
    pivotTable.AddFieldToArea(PivotFieldType.Data, "Incurred");


    //Calculated fields
    pivotTable.AddCalculatedField("Inc to Earned LR", "('Incurred'/'Earned')");

    pivotTable.AddFieldToArea(PivotFieldType.Column, pivotTable.DataField);

    //Update Captions and NumberFormats
    pivotDataFields = pivotTable.DataFields;

    pivotDataFields["Written"].DisplayName = "Written";
    pivotDataFields["Written"].NumberFormat = @"_($* #,##0.00_);_($* (#,##0.00);_($* "" - ""??_);_(@_)";

    pivotDataFields["Earned"].DisplayName = "Earned";
    pivotDataFields["Earned"].NumberFormat = @"_($* #,##0.00_);_($* (#,##0.00);_($* "" - ""??_);_(@_)";

    pivotDataFields["Incurred"].DisplayName = "Incurred";
    pivotDataFields["Incurred"].NumberFormat = @"_($* #,##0.00_);_($* (#,##0.00);_($* "" - ""??_);_(@_)";

    pivotDataFields["Inc to Earned LR"].DisplayName = "Inc to Earned LR %";
    pivotDataFields["Inc to Earned LR"].NumberFormat = "0.00%";


    //Conditional format Loss Ratio >= 40%
    PivotConditionalFormatCollection pcfCollection = pivotTable.ConditionalFormats;
    pcfCollection.Clear();
    worksheet.ConditionalFormattings.Clear();

    PivotConditionalFormat pcf = pcfCollection[pcfCollection.Add()];
    pcf.ScopeType = PivotConditionFormatScopeType.Field;

    PivotArea pivotArea = new PivotArea(pivotTable);
    pivotArea.SelectField(PivotFieldType.Data, "Inc to Earned LR");
    pivotArea.SelectField(PivotFieldType.Row, "CommonName");
    pcf.PivotAreas.Add(pivotArea);
    Assert.IsTrue(pivotArea.Filters[1].IsSubtotalSet(PivotFieldSubtotalType.Automatic));

    //pcf.AddFieldArea(PivotFieldType.Data, "Inc to Earned LR");
    //pcf.AddFieldArea(PivotFieldType.Row, "CommonName");

    FormatConditionCollection fcc = pcf.FormatConditions;
    int idx = fcc.AddCondition(FormatConditionType.CellValue);
    FormatCondition fc = fcc[idx];
    fc.Formula1 = "0.4";
    fc.Operator = OperatorType.GreaterOrEqual;
    fc.Style.BackgroundArgbColor = Color.FromArgb(255, 199, 206).ToArgb();
    fc.Style.Font.ArgbColor = Color.FromArgb(156, 0, 6).ToArgb();


    pivotTable.RefreshData();
    pivotTable.CalculateData();
    pivotTable.RefreshDataOnOpeningFile = true;

    //Autofit all columns and rows
    worksheet.AutoFitColumns();
    worksheet.AutoFitRows();
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## SelectField(PivotFieldType, PivotField) {#selectfield}

Select a field in the region as an area.

```csharp
public void SelectField(PivotFieldType axisType, PivotField field)
```

| Parameter | Type | Description |
| --- | --- | --- |
| axisType | PivotFieldType | The region type. |
| field | PivotField | The pivot field. |

### Examples

```csharp
// Called: pivotArea.SelectField(PivotFieldType.Data, excelPivot.DataFields[0]);
        public void PivotArea_Method_SelectField()
        {
            byte[] SrcDataByteArray = Encoding.ASCII.GetBytes(
 $@"City,Product,Sales
Paris,Cream,2300
Paris,Lotion,1600
Tunis,Cream,900
Tunis,Lotion,1400
Tunis,Cream,3090
Tunis,Lotion,6000
Paris,Cream,4320");

            // Create a memory stream from the source data
            MemoryStream dataStream = new MemoryStream(SrcDataByteArray);

            // Create LoadOptions class object to load the comma-separated data given above
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Csv);

            // Instantiate a workbook class object having above mentioned data
            Workbook wbCSV = new Workbook(dataStream, loadOptions);

            // Get access to the first worksheet in the collection
            Worksheet targetSheet = wbCSV.Worksheets[0];

            // Get collection of pivot tables in the target worksheet
            Aspose.Cells.Pivot.PivotTableCollection pvTablesCollection = targetSheet.PivotTables;

            // Get pivot table index after adding a new pivot table by provding source data range and destination cell
            int iNewPivotTable = pvTablesCollection.Add("=A1:C8", "F3", "MyPivotTable");

            // Get the instance of newly added pivot table for further processing
            Aspose.Cells.Pivot.PivotTable excelPivot = pvTablesCollection[iNewPivotTable];

            // Hide the grand total for rows in the output Excel file
            excelPivot.ShowRowGrandTotals = false;
            excelPivot.ShowColumnGrandTotals = false;

            // Add the first field to the column area
            excelPivot.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Column, 0);
            // Add the second field to the row area
            excelPivot.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, 1);
            // Add the third field to the data area
            excelPivot.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, 2);


            // Conditional formatting

            //int ind = targetSheet.ConditionalFormattings.Add();
            //FormatConditionCollection fcs = targetSheet.ConditionalFormattings[ind];
            //CellArea cellArea = new CellArea()
            //{
            //    StartRow = 1,
            //    EndRow = 7,
            //    StartColumn = 2,
            //    EndColumn = 2
            //};
            //fcs.AddArea(cellArea);

            //int indexCond = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "1", null);
            //fcs[indexCond].Style.BackgroundColor = ColorTranslator.FromHtml("#e39e9e");



            int ind = excelPivot.ConditionalFormats.Add();
            PivotConditionalFormat pivForCond = excelPivot.ConditionalFormats[ind];
            pivForCond.ScopeType = PivotConditionFormatScopeType.Data;
            //pivForCond.AddDataAreaCondition(excelPivot.DataFields[0]);

            PivotArea pivotArea = new PivotArea(excelPivot);
            pivotArea.SelectField(PivotFieldType.Data, excelPivot.DataFields[0]);
            pivForCond.PivotAreas.Add(pivotArea);

            int indexCond = pivForCond.FormatConditions.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "1", null);
            pivForCond.FormatConditions[indexCond].Style.BackgroundColor = ColorTranslator.FromHtml("#e39e9e");
            pivForCond.FormatConditions.AddArea(excelPivot.DataBodyRange);
            //excelPivot.RefreshData();
            //excelPivot.CalculateData();
            //pivForCond.SetConditionalAreas();


            // Saving the output Excel file with pivot table
            wbCSV.Save(Constants.PivotTableDestPath + "example.xlsx");
            wbCSV = new Workbook(Constants.PivotTableDestPath + "example.xlsx");
            Assert.AreEqual(1, wbCSV.Worksheets[0].ConditionalFormattings.Count);

            System.Console.WriteLine("Done");
        }
```

### See Also

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotField](../../pivotfield/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


