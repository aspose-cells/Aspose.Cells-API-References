---
title: PivotConditionalFormat.AddFieldArea
second_title: Aspose.Cells for .NET API Reference
description: PivotConditionalFormat method. Adds an area of pivot field
type: docs
url: /net/aspose.cells.pivot/pivotconditionalformat/addfieldarea/
---
## AddFieldArea(PivotFieldType, string) {#addfieldarea_1}

Adds an area of pivot field.

```csharp
public void AddFieldArea(PivotFieldType axisType, string fieldName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| axisType | PivotFieldType | The region type. |
| fieldName | String | The name of pivot field. |

### Examples

```csharp
// Called: pcf.AddFieldArea(PivotFieldType.Row, &amp;quot;CommonName&amp;quot;);
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

            //PivotArea pivotArea = new PivotArea(pivotTable);
            //pivotArea.SelectField(PivotFieldType.Data, &quot;Inc to Earned LR&quot;);
            //pivotArea.SelectField(PivotFieldType.Row, &quot;CommonName&quot;);
            //pcf.PivotAreas.Add(pivotArea);


            pcf.AddFieldArea(PivotFieldType.Data, &quot;Inc to Earned LR&quot;);
            pcf.AddFieldArea(PivotFieldType.Row, &quot;CommonName&quot;);
            Assert.IsTrue(pcf.PivotAreas[0].Filters[1].IsSubtotalSet(PivotFieldSubtotalType.Automatic));
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
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## AddFieldArea(PivotFieldType, PivotField) {#addfieldarea}

Adds an area of pivot field.

```csharp
public void AddFieldArea(PivotFieldType axisType, PivotField field)
```

| Parameter | Type | Description |
| --- | --- | --- |
| axisType | PivotFieldType | The region type. |
| field | PivotField | The pivot field. |

### Examples

```csharp
// Called: pfc.AddFieldArea(PivotFieldType.Row, pivot.RowFields[0]);
[Test]
        public void Method_PivotField_()
        {
            Workbook book = new Workbook();

            PivotTable pivot = CreateATable(book);
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            //Add PivotFormatCondition
            int formatIndex = pivot.ConditionalFormats.Add();
            PivotConditionalFormat pfc = pivot.ConditionalFormats[formatIndex];
            //int formatIndex = pivot.PivotFormatConditions.Add();
            //PivotFormatCondition pfc = pivot.PivotFormatConditions[formatIndex];
            pfc.AddFieldArea(PivotFieldType.Row, pivot.RowFields[0]);
            FormatConditionCollection fcc = pfc.FormatConditions;
            CellArea ca = fcc.GetCellArea(0);
            Assert.IsTrue(CellAreaTest.equals(ca, CellArea.CreateCellArea(&quot;B14&quot;, &quot;D17&quot;), &quot;Area&quot;));

            int index = pfc.FormatConditions.AddCondition(FormatConditionType.CellValue);
            FormatCondition fc = pfc.FormatConditions[index];
            fc.Formula1 = &quot;100&quot;;
            fc.Operator = OperatorType.GreaterOrEqual;
            fc.Style.BackgroundColor = Color.Red;
            book.Save(Constants.destPath + &quot;CellsNet57427_2.xlsx&quot;);

        }
```

### See Also

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotField](../../pivotfield/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


