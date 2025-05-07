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
// Called: pcf.AddFieldArea(PivotFieldType.Data, "Inc to Earned LR");
[Test]
        public void Method_String_()
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

            //PivotArea pivotArea = new PivotArea(pivotTable);
            //pivotArea.SelectField(PivotFieldType.Data, "Inc to Earned LR");
            //pivotArea.SelectField(PivotFieldType.Row, "CommonName");
            //pcf.PivotAreas.Add(pivotArea);


            pcf.AddFieldArea(PivotFieldType.Data, "Inc to Earned LR");
            pcf.AddFieldArea(PivotFieldType.Row, "CommonName");
            Assert.IsTrue(pcf.PivotAreas[0].Filters[1].IsSubtotalSet(PivotFieldSubtotalType.Automatic));
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
            Assert.IsTrue(CellAreaTest.equals(ca, CellArea.CreateCellArea("B14", "D17"), "Area"));

            int index = pfc.FormatConditions.AddCondition(FormatConditionType.CellValue);
            FormatCondition fc = pfc.FormatConditions[index];
            fc.Formula1 = "100";
            fc.Operator = OperatorType.GreaterOrEqual;
            fc.Style.BackgroundColor = Color.Red;
            book.Save(Constants.destPath + "CellsNet57427_2.xlsx");

        }
```

### See Also

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotField](../../pivotfield/)
* class [PivotConditionalFormat](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


