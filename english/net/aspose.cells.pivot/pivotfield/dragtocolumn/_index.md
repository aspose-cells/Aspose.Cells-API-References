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
private void PivotField_Property_DragToColumn(DataTable data, string filePath)
        {
            var workbook = new Workbook();
#if NETCOREAPP2_0
            workbook.Settings.CultureInfo = new System.Globalization.CultureInfo("en-US");
#endif
            var dataSourceWorksheet = workbook.Worksheets.Add("Data");
            dataSourceWorksheet.Cells.ImportData(data, 0, 0, new ImportTableOptions() { IsFieldNameShown = true });

            var pivotWorksheet = workbook.Worksheets.Add("PivotTable");

            // Title
            var titleCell = pivotWorksheet.Cells["E2"];
            var style = titleCell.GetStyle();
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = Color.FromArgb(150, 54, 52);
            style.BackgroundColor = style.ForegroundColor;
            style.Font.Size = 22;
            style.Font.Name = "Calibri";
            style.Font.Color = Color.White;
            titleCell.SetStyle(style);

            pivotWorksheet.Cells["E2"].PutValue("Synthesis FO");
            pivotWorksheet.Cells.Merge(1, 4, 4, 3);

            pivotWorksheet.IsGridlinesVisible = false;
            pivotWorksheet.AutoFitColumns();

            // Pivot Table
            int index = pivotWorksheet.PivotTables.Add("=Data!A1:N411", "B7", "PivotTable");
            //int index = pivotWorksheet.PivotTables.Add("=Data!A1:L10", "B7", "PivotTable");//NET46734
            var pivotTable = pivotWorksheet.PivotTables[index];
            //workbook.Save(CreateFolder(filePath) + "out_data2.xlsx");

            // Rows
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Desk");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Action");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "ExDate");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "OstType");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "ReInvestFacility");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "CodeBBG");

            // Data
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Size");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "SizeTd");

            // Filters
            pivotTable.AddFieldToArea(PivotFieldType.Page, "LockedPtf");
            pivotTable.AddFieldToArea(PivotFieldType.Page, "ExcludedOstType");
            pivotTable.AddFieldToArea(PivotFieldType.Page, "DiffExDate");
            pivotTable.AddFieldToArea(PivotFieldType.Page, "Message");

            // Columns
            pivotTable.AddFieldToArea(PivotFieldType.Column, pivotTable.DataField);

            var deskField = pivotTable.RowFields["Desk"];
            deskField.SetSubtotals(PivotFieldSubtotalType.None, true);
            deskField.InsertBlankRow = true;
            deskField.ShowInOutlineForm = false;
            deskField.IsAutoSort = true;
            deskField.IsAscendSort = true;

            var actionField = pivotTable.RowFields["Action"];
            actionField.SetSubtotals(PivotFieldSubtotalType.None, true);
            actionField.InsertBlankRow = true;
            actionField.ShowInOutlineForm = true;
            actionField.ShowCompact = true;

            var exDateField = pivotTable.RowFields["ExDate"];
            exDateField.SetSubtotals(PivotFieldSubtotalType.None, true);
            exDateField.InsertBlankRow = false;
            exDateField.ShowInOutlineForm = false;
            exDateField.IsAutoSort = true;
            exDateField.IsAscendSort = true;
            exDateField.NumberFormat = "dd-mmm-yy";

            var ostTypeField = pivotTable.RowFields["OstType"];
            ostTypeField.SetSubtotals(PivotFieldSubtotalType.None, true);
            ostTypeField.InsertBlankRow = false;
            ostTypeField.ShowInOutlineForm = false;

            var reifField = pivotTable.RowFields["ReInvestFacility"];
            reifField.SetSubtotals(PivotFieldSubtotalType.None, true);
            reifField.InsertBlankRow = false;
            reifField.ShowInOutlineForm = false;

            var codeBBGField = pivotTable.RowFields["CodeBBG"];
            codeBBGField.SetSubtotals(PivotFieldSubtotalType.None, true);
            codeBBGField.ShowInOutlineForm = false;
            codeBBGField.IsAutoSort = true;
            codeBBGField.IsAscendSort = true;
            codeBBGField.InsertBlankRow = false;

            var sizeField = pivotTable.DataFields["Size"];
            sizeField.DragToColumn = true;
            sizeField.DisplayName = "Size";
            sizeField.NumberFormat = "#,##0";

            var sizeTdField = pivotTable.DataFields["SizeTd"];
            sizeTdField.DragToColumn = true;
            sizeTdField.DisplayName = "SizeTd";
            sizeTdField.NumberFormat = "#,##0";

            pivotTable.PageFields["LockedPtf"].CurrentPageItem = 0;
            pivotTable.PageFields["ExcludedOstType"].CurrentPageItem = 1;
            //pivotTable.PageFields["ExcludedOstType"].CurrentPageItem = 0;//for NET46734
            pivotTable.PageFields["Message"].CurrentPageItem = 0;

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
            Assert.AreEqual(cells["C10"].StringValue, "04-Feb-16");
            Assert.AreEqual(cells["C13"].StringValue, "08-Feb-16");
            Assert.AreEqual("Row Labels", cells["B8"].StringValue);
            Assert.AreEqual("Data", cells["G7"].StringValue);
            workbook.Save(CreateFolder(filePath) + "out_pivot.xlsx", SaveFormat.Xlsx);
            workbook.Save(CreateFolder(filePath) + "out.html", new HtmlSaveOptions(SaveFormat.Html) { ExportActiveWorksheetOnly = true });
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


