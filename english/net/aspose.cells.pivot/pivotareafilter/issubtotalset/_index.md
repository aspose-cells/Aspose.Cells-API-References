---
title: PivotAreaFilter.IsSubtotalSet
second_title: Aspose.Cells for .NET API Reference
description: PivotAreaFilter method. Gets which subtotal is set for this filter
type: docs
url: /net/aspose.cells.pivot/pivotareafilter/issubtotalset/
---
## PivotAreaFilter.IsSubtotalSet method

Gets which subtotal is set for this filter.

```csharp
public bool IsSubtotalSet(PivotFieldSubtotalType subtotalType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| subtotalType | PivotFieldSubtotalType | The subtotal function type. |

### Examples

```csharp
// Called: Assert.IsTrue(pivotArea.Filters[1].IsSubtotalSet(PivotFieldSubtotalType.Automatic));
[Test]
        public void Method_PivotFieldSubtotalType_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet57743.xlsx");
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
            workbook.Save(Constants.destPath + "CellsNet57743.xlsx");
        }
```

### See Also

* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotAreaFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


