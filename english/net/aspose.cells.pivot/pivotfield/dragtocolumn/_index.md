---
title: PivotField.DragToColumn
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Indicates whether the specified field can be dragged to the column position. The default value is true
type: docs
url: /net/aspose.cells.pivot/pivotfield/dragtocolumn/
---
## PivotField.DragToColumn property

Indicates whether the specified field can be dragged to the column position. The default value is true.

```csharp
public bool DragToColumn { get; set; }
```

### Examples

```csharp
// Called: sizeField.DragToColumn = true;
private void Property_DragToColumn(DataTable data, string filePath)
        {
            var workbook = new Workbook();
#if NETCOREAPP2_0
            workbook.Settings.CultureInfo = new System.Globalization.CultureInfo(&quot;en-US&quot;);
#endif
            var dataSourceWorksheet = workbook.Worksheets.Add(&quot;Data&quot;);
            dataSourceWorksheet.Cells.ImportData(data, 0, 0, new ImportTableOptions() { IsFieldNameShown = true });

            var pivotWorksheet = workbook.Worksheets.Add(&quot;PivotTable&quot;);

            // Title
            var titleCell = pivotWorksheet.Cells[&quot;E2&quot;];
            var style = titleCell.GetStyle();
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = Color.FromArgb(150, 54, 52);
            style.BackgroundColor = style.ForegroundColor;
            style.Font.Size = 22;
            style.Font.Name = &quot;Calibri&quot;;
            style.Font.Color = Color.White;
            titleCell.SetStyle(style);

            pivotWorksheet.Cells[&quot;E2&quot;].PutValue(&quot;Synthesis FO&quot;);
            pivotWorksheet.Cells.Merge(1, 4, 4, 3);

            pivotWorksheet.IsGridlinesVisible = false;
            pivotWorksheet.AutoFitColumns();

            // Pivot Table
            int index = pivotWorksheet.PivotTables.Add(&quot;=Data!A1:N411&quot;, &quot;B7&quot;, &quot;PivotTable&quot;);
            //int index = pivotWorksheet.PivotTables.Add(&quot;=Data!A1:L10&quot;, &quot;B7&quot;, &quot;PivotTable&quot;);//NET46734
            var pivotTable = pivotWorksheet.PivotTables[index];
            //workbook.Save(CreateFolder(filePath) + &quot;out_data2.xlsx&quot;);

            // Rows
            pivotTable.AddFieldToArea(PivotFieldType.Row, &quot;Desk&quot;);
            pivotTable.AddFieldToArea(PivotFieldType.Row, &quot;Action&quot;);
            pivotTable.AddFieldToArea(PivotFieldType.Row, &quot;ExDate&quot;);
            pivotTable.AddFieldToArea(PivotFieldType.Row, &quot;OstType&quot;);
            pivotTable.AddFieldToArea(PivotFieldType.Row, &quot;ReInvestFacility&quot;);
            pivotTable.AddFieldToArea(PivotFieldType.Row, &quot;CodeBBG&quot;);

            // Data
            pivotTable.AddFieldToArea(PivotFieldType.Data, &quot;Size&quot;);
            pivotTable.AddFieldToArea(PivotFieldType.Data, &quot;SizeTd&quot;);

            // Filters
            pivotTable.AddFieldToArea(PivotFieldType.Page, &quot;LockedPtf&quot;);
            pivotTable.AddFieldToArea(PivotFieldType.Page, &quot;ExcludedOstType&quot;);
            pivotTable.AddFieldToArea(PivotFieldType.Page, &quot;DiffExDate&quot;);
            pivotTable.AddFieldToArea(PivotFieldType.Page, &quot;Message&quot;);

            // Columns
            pivotTable.AddFieldToArea(PivotFieldType.Column, pivotTable.DataField);

            var deskField = pivotTable.RowFields[&quot;Desk&quot;];
            deskField.SetSubtotals(PivotFieldSubtotalType.None, true);
            deskField.InsertBlankRow = true;
            deskField.ShowInOutlineForm = false;
            deskField.IsAutoSort = true;
            deskField.IsAscendSort = true;

            var actionField = pivotTable.RowFields[&quot;Action&quot;];
            actionField.SetSubtotals(PivotFieldSubtotalType.None, true);
            actionField.InsertBlankRow = true;
            actionField.ShowInOutlineForm = true;
            actionField.ShowCompact = true;

            var exDateField = pivotTable.RowFields[&quot;ExDate&quot;];
            exDateField.SetSubtotals(PivotFieldSubtotalType.None, true);
            exDateField.InsertBlankRow = false;
            exDateField.ShowInOutlineForm = false;
            exDateField.IsAutoSort = true;
            exDateField.IsAscendSort = true;
            exDateField.NumberFormat = &quot;dd-mmm-yy&quot;;

            var ostTypeField = pivotTable.RowFields[&quot;OstType&quot;];
            ostTypeField.SetSubtotals(PivotFieldSubtotalType.None, true);
            ostTypeField.InsertBlankRow = false;
            ostTypeField.ShowInOutlineForm = false;

            var reifField = pivotTable.RowFields[&quot;ReInvestFacility&quot;];
            reifField.SetSubtotals(PivotFieldSubtotalType.None, true);
            reifField.InsertBlankRow = false;
            reifField.ShowInOutlineForm = false;

            var codeBBGField = pivotTable.RowFields[&quot;CodeBBG&quot;];
            codeBBGField.SetSubtotals(PivotFieldSubtotalType.None, true);
            codeBBGField.ShowInOutlineForm = false;
            codeBBGField.IsAutoSort = true;
            codeBBGField.IsAscendSort = true;
            codeBBGField.InsertBlankRow = false;

            var sizeField = pivotTable.DataFields[&quot;Size&quot;];
            sizeField.DragToColumn = true;
            sizeField.DisplayName = &quot;Size&quot;;
            sizeField.NumberFormat = &quot;#,##0&quot;;

            var sizeTdField = pivotTable.DataFields[&quot;SizeTd&quot;];
            sizeTdField.DragToColumn = true;
            sizeTdField.DisplayName = &quot;SizeTd&quot;;
            sizeTdField.NumberFormat = &quot;#,##0&quot;;

            pivotTable.PageFields[&quot;LockedPtf&quot;].CurrentPageItem = 0;
            pivotTable.PageFields[&quot;ExcludedOstType&quot;].CurrentPageItem = 1;
            //pivotTable.PageFields[&quot;ExcludedOstType&quot;].CurrentPageItem = 0;//for NET46734
            pivotTable.PageFields[&quot;Message&quot;].CurrentPageItem = 0;

            pivotTable.IsAutoFormat = true;
            pivotTable.AutoFormatType = PivotTableAutoFormatType.Classic;
            pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium3;
            pivotTable.ShowDrill = false;
            pivotTable.ShowRowGrandTotals = false;
            pivotTable.ShowColumnGrandTotals = false;

            pivotTable.RefreshData();
            pivotTable.CalculateData();
            pivotTable.RefreshDataOnOpeningFile = false;

            workbook.Worksheets.ActiveSheetIndex = pivotWorksheet.Index;

            Cells cells = workbook.Worksheets[pivotWorksheet.Index].Cells;
            Assert.AreEqual(cells[&quot;C10&quot;].StringValue, &quot;04-Feb-16&quot;);
            Assert.AreEqual(cells[&quot;C13&quot;].StringValue, &quot;08-Feb-16&quot;);
            Assert.AreEqual(&quot;Row Labels&quot;, cells[&quot;B8&quot;].StringValue);
            Assert.AreEqual(&quot;Data&quot;, cells[&quot;G7&quot;].StringValue);
            workbook.Save(CreateFolder(filePath) + &quot;out_pivot.xlsx&quot;, SaveFormat.Xlsx);
            workbook.Save(CreateFolder(filePath) + &quot;out.html&quot;, new HtmlSaveOptions(SaveFormat.Html) { ExportActiveWorksheetOnly = true });
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


