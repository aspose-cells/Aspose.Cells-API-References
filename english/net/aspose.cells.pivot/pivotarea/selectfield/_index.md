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
// Called: pivotArea.SelectField(PivotFieldType.Row, &amp;quot;CommonName&amp;quot;);
[Test]
        public void Method_String_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet57743.xlsx&quot;);
            PivotTableCollection pivotTables;
            PivotTable pivotTable;
            PivotField pivotField;
            PivotItemCollection pivotItems;
            PivotItem pivotItem;
            PivotFieldCollection pivotDataFields;

            int pivotTableIndex;

            Worksheet detailWorksheet = workbook.Worksheets[&quot;Detail&quot;];


            Worksheet worksheet = workbook.Worksheets.Add(&quot;RENEWALS WITH LR &gt;= 40%&quot;);
            worksheet.TabColor = Color.Red;

            pivotTables = worksheet.PivotTables;

            pivotTableIndex = pivotTables.Add($&quot;&apos;Detail&apos;!A1:{CellsHelper.CellIndexToName(detailWorksheet.Cells.MaxDataRow, detailWorksheet.Cells.MaxDataColumn)}&quot;, &quot;A1&quot;, &quot;PivotTable1&quot;);

            pivotTable = pivotTables[pivotTableIndex];

            pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleLight16;

            pivotTable.ShowValuesRow = false;

            //RowFields
            pivotTable.AddFieldToArea(PivotFieldType.Row, &quot;MonthDay&quot;);

            //Uncheck &quot;(blank)&quot; item
            pivotField = pivotTable.RowFields[&quot;MonthDay&quot;];
            pivotField.IsAutoSort = true;
            pivotField.IsAscendSort = true;

            pivotItems = pivotField.PivotItems;

            for (int i = 0; i &lt; pivotItems.Count; i++)
            {
                pivotItem = pivotItems[i];
                if (pivotItem.Name != null &amp;&amp; pivotItem.Name.Equals(&quot;(blank)&quot;))
                {
                    pivotItem.IsHidden = true;
                }
            }

            pivotTable.AddFieldToArea(PivotFieldType.Row, &quot;CommonName&quot;);

            pivotTable.AddFieldToArea(PivotFieldType.Row, &quot;PolicyNumber&quot;);
            pivotField = pivotTable.RowFields[&quot;PolicyNumber&quot;];
            //Hide Subtotal
            pivotField.IsAutoSubtotals = false;

            pivotTable.AddFieldToArea(PivotFieldType.Row, &quot;CoveragePart&quot;);
            pivotField = pivotTable.RowFields[&quot;CoveragePart&quot;];
            //Hide Subtotal
            pivotField.IsAutoSubtotals = false;

            pivotTable.AddFieldToArea(PivotFieldType.Row, &quot;ExpDate&quot;);
            pivotField = pivotTable.RowFields[&quot;ExpDate&quot;];
            //Hide Subtotal
            pivotField.IsAutoSubtotals = false;

            pivotTable.AddFieldToArea(PivotFieldType.Row, &quot;ClaimCount&quot;);

            //DataFields
            pivotTable.AddFieldToArea(PivotFieldType.Data, &quot;Written&quot;);
            pivotTable.AddFieldToArea(PivotFieldType.Data, &quot;Earned&quot;);
            pivotTable.AddFieldToArea(PivotFieldType.Data, &quot;Incurred&quot;);


            //Calculated fields
            pivotTable.AddCalculatedField(&quot;Inc to Earned LR&quot;, &quot;(&apos;Incurred&apos;/&apos;Earned&apos;)&quot;);

            pivotTable.AddFieldToArea(PivotFieldType.Column, pivotTable.DataField);

            //Update Captions and NumberFormats
            pivotDataFields = pivotTable.DataFields;

            pivotDataFields[&quot;Written&quot;].DisplayName = &quot;Written&quot;;
            pivotDataFields[&quot;Written&quot;].NumberFormat = @&quot;_($* #,##0.00_);_($* (#,##0.00);_($* &quot;&quot; - &quot;&quot;??_);_(@_)&quot;;

            pivotDataFields[&quot;Earned&quot;].DisplayName = &quot;Earned&quot;;
            pivotDataFields[&quot;Earned&quot;].NumberFormat = @&quot;_($* #,##0.00_);_($* (#,##0.00);_($* &quot;&quot; - &quot;&quot;??_);_(@_)&quot;;

            pivotDataFields[&quot;Incurred&quot;].DisplayName = &quot;Incurred&quot;;
            pivotDataFields[&quot;Incurred&quot;].NumberFormat = @&quot;_($* #,##0.00_);_($* (#,##0.00);_($* &quot;&quot; - &quot;&quot;??_);_(@_)&quot;;

            pivotDataFields[&quot;Inc to Earned LR&quot;].DisplayName = &quot;Inc to Earned LR %&quot;;
            pivotDataFields[&quot;Inc to Earned LR&quot;].NumberFormat = &quot;0.00%&quot;;


            //Conditional format Loss Ratio &gt;= 40%
            PivotConditionalFormatCollection pcfCollection = pivotTable.ConditionalFormats;
            pcfCollection.Clear();
            worksheet.ConditionalFormattings.Clear();

            PivotConditionalFormat pcf = pcfCollection[pcfCollection.Add()];
            pcf.ScopeType = PivotConditionFormatScopeType.Field;

            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.SelectField(PivotFieldType.Data, &quot;Inc to Earned LR&quot;);
            pivotArea.SelectField(PivotFieldType.Row, &quot;CommonName&quot;);
            pcf.PivotAreas.Add(pivotArea);
            Assert.IsTrue(pivotArea.Filters[1].IsSubtotalSet(PivotFieldSubtotalType.Automatic));

            //pcf.AddFieldArea(PivotFieldType.Data, &quot;Inc to Earned LR&quot;);
            //pcf.AddFieldArea(PivotFieldType.Row, &quot;CommonName&quot;);

            FormatConditionCollection fcc = pcf.FormatConditions;
            int idx = fcc.AddCondition(FormatConditionType.CellValue);
            FormatCondition fc = fcc[idx];
            fc.Formula1 = &quot;0.4&quot;;
            fc.Operator = OperatorType.GreaterOrEqual;
            fc.Style.BackgroundArgbColor = Color.FromArgb(255, 199, 206).ToArgb();
            fc.Style.Font.ArgbColor = Color.FromArgb(156, 0, 6).ToArgb();


            pivotTable.RefreshData();
            pivotTable.CalculateData();
            pivotTable.RefreshDataOnOpeningFile = true;

            //Autofit all columns and rows
            worksheet.AutoFitColumns();
            worksheet.AutoFitRows();
            workbook.Save(Constants.destPath + &quot;CellsNet57743.xlsx&quot;);
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
[Test]
        public void Method_PivotField_()
        {
            byte[] SrcDataByteArray = Encoding.ASCII.GetBytes(
 $@&quot;City,Product,Sales
Paris,Cream,2300
Paris,Lotion,1600
Tunis,Cream,900
Tunis,Lotion,1400
Tunis,Cream,3090
Tunis,Lotion,6000
Paris,Cream,4320&quot;);

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
            int iNewPivotTable = pvTablesCollection.Add(&quot;=A1:C8&quot;, &quot;F3&quot;, &quot;MyPivotTable&quot;);

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

            //int indexCond = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, &quot;1&quot;, null);
            //fcs[indexCond].Style.BackgroundColor = ColorTranslator.FromHtml(&quot;#e39e9e&quot;);



            int ind = excelPivot.ConditionalFormats.Add();
            PivotConditionalFormat pivForCond = excelPivot.ConditionalFormats[ind];
            pivForCond.ScopeType = PivotConditionFormatScopeType.Data;
            //pivForCond.AddDataAreaCondition(excelPivot.DataFields[0]);

            PivotArea pivotArea = new PivotArea(excelPivot);
            pivotArea.SelectField(PivotFieldType.Data, excelPivot.DataFields[0]);
            pivForCond.PivotAreas.Add(pivotArea);

            int indexCond = pivForCond.FormatConditions.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, &quot;1&quot;, null);
            pivForCond.FormatConditions[indexCond].Style.BackgroundColor = ColorTranslator.FromHtml(&quot;#e39e9e&quot;);
            pivForCond.FormatConditions.AddArea(excelPivot.DataBodyRange);
            //excelPivot.RefreshData();
            //excelPivot.CalculateData();
            //pivForCond.SetConditionalAreas();


            // Saving the output Excel file with pivot table
            wbCSV.Save(Constants.PivotTableDestPath + &quot;CELLSNET-57427.xlsx&quot;);
            wbCSV = new Workbook(Constants.PivotTableDestPath + &quot;CELLSNET-57427.xlsx&quot;);
            Assert.AreEqual(1, wbCSV.Worksheets[0].ConditionalFormattings.Count);

            System.Console.WriteLine(&quot;Done&quot;);
        }
```

### See Also

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotField](../../pivotfield/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


