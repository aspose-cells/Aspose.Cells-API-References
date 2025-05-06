---
title: PivotConditionalFormat.ScopeType
second_title: Aspose.Cells for .NET API Reference
description: PivotConditionalFormat property. Get and set scope type for the pivot table conditional format 
type: docs
url: /net/aspose.cells.pivot/pivotconditionalformat/scopetype/
---
## PivotConditionalFormat.ScopeType property

Get and set scope type for the pivot table conditional format .

```csharp
public PivotConditionFormatScopeType ScopeType { get; set; }
```

### Examples

```csharp
// Called: pcf.ScopeType = PivotConditionFormatScopeType.Field;
[Test]
        public void Property_ScopeType()
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

* enum [PivotConditionFormatScopeType](../../pivotconditionformatscopetype/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


