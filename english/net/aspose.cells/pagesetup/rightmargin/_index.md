---
title: PageSetup.RightMargin
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Represents the size of the right margin in unit of centimeters
type: docs
url: /net/aspose.cells/pagesetup/rightmargin/
---
## PageSetup.RightMargin property

Represents the size of the right margin, in unit of centimeters.

```csharp
public double RightMargin { get; set; }
```

### Examples

```csharp
// Called: ws.PageSetup.RightMargin = 0;
        public void PageSetup_Property_RightMargin()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @"NET45262/";

            string savePath = CreateFolder(filePath);
            Workbook wb = null;
            Worksheet ws = null;
            Style style = null;
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Borders = true;
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportActiveWorksheetOnly = true;
#region default
            wb = new Workbook(filePath + "input.xlsx");
            ws = wb.Worksheets[0];
            wb.Worksheets.ActiveSheetIndex = 0;
            //render whole worksheet
            ws.PageSetup.BottomMargin = 0;
            ws.PageSetup.LeftMargin = 0;
            ws.PageSetup.RightMargin = 0;
            ws.PageSetup.TopMargin = 0;
            ws.PageSetup.PrintArea = string.Empty;

            options.HtmlCrossStringType = HtmlCrossType.Default;
            wb.Save(savePath + "default_noBorder.html", options);

            wb = new Workbook(filePath + "input.xlsx");
            ws = wb.Worksheets[0];
            wb.Worksheets.ActiveSheetIndex = 0;
            //render whole worksheet
            ws.PageSetup.BottomMargin = 0;
            ws.PageSetup.LeftMargin = 0;
            ws.PageSetup.RightMargin = 0;
            ws.PageSetup.TopMargin = 0;
            ws.PageSetup.PrintArea = string.Empty;

            options.HtmlCrossStringType = HtmlCrossType.Default;
            //show grid lines
            style = wb.CreateStyle();
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

            ws.Cells.MaxDisplayRange.ApplyStyle(style, styleFlag);

            options.HtmlCrossStringType = HtmlCrossType.Default;
            wb.Save(savePath + "default_border.html", options);
#endregion

#region cross
            wb = new Workbook(filePath + "input.xlsx");
            ws = wb.Worksheets[0];
            wb.Worksheets.ActiveSheetIndex = 0;
            //render whole worksheet
            ws.PageSetup.BottomMargin = 0;
            ws.PageSetup.LeftMargin = 0;
            ws.PageSetup.RightMargin = 0;
            ws.PageSetup.TopMargin = 0;
            ws.PageSetup.PrintArea = string.Empty;

            options.HtmlCrossStringType = HtmlCrossType.Cross;
            wb.Save(savePath + "cross_noBorder.html", options);

            wb = new Workbook(filePath + "input.xlsx");
            ws = wb.Worksheets[0];
            wb.Worksheets.ActiveSheetIndex = 0;
            //render whole worksheet
            ws.PageSetup.BottomMargin = 0;
            ws.PageSetup.LeftMargin = 0;
            ws.PageSetup.RightMargin = 0;
            ws.PageSetup.TopMargin = 0;
            ws.PageSetup.PrintArea = string.Empty;


            options.HtmlCrossStringType = HtmlCrossType.Default;
            //show grid lines
            style = wb.CreateStyle();
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;


            ws.Cells.MaxDisplayRange.ApplyStyle(style, styleFlag);
            options.HtmlCrossStringType = HtmlCrossType.Cross;
            wb.Save(savePath + "cross_border.html", options);
#endregion

#region fitToCell
            wb = new Workbook(filePath + "input-fit.xlsx");
            ws = wb.Worksheets[0];
            wb.Worksheets.ActiveSheetIndex = 0;
            //render whole worksheet
            ws.PageSetup.BottomMargin = 0;
            ws.PageSetup.LeftMargin = 0;
            ws.PageSetup.RightMargin = 0;
            ws.PageSetup.TopMargin = 0;
            ws.PageSetup.PrintArea = string.Empty;

            options.HtmlCrossStringType = HtmlCrossType.FitToCell;
            wb.Save(savePath + "fitToCell_noBorder.html", options);

            wb = new Workbook(filePath + "input-fit.xlsx");
            ws = wb.Worksheets[0];
            wb.Worksheets.ActiveSheetIndex = 0;
            //render whole worksheet
            ws.PageSetup.BottomMargin = 0;
            ws.PageSetup.LeftMargin = 0;
            ws.PageSetup.RightMargin = 0;
            ws.PageSetup.TopMargin = 0;
            ws.PageSetup.PrintArea = string.Empty;

            options.HtmlCrossStringType = HtmlCrossType.Default;
            //show grid lines
            style = wb.CreateStyle();
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;

            ws.Cells.MaxDisplayRange.ApplyStyle(style, styleFlag);

            options.HtmlCrossStringType = HtmlCrossType.FitToCell;
            wb.Save(savePath + "fitToCell_border.html", options);
#endregion

        }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


