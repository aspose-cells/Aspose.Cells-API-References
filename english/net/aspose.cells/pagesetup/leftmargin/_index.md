---
title: PageSetup.LeftMargin
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Represents the size of the left margin in unit of centimeters
type: docs
url: /net/aspose.cells/pagesetup/leftmargin/
---
## PageSetup.LeftMargin property

Represents the size of the left margin, in unit of centimeters.

```csharp
public double LeftMargin { get; set; }
```

### Examples

```csharp
// Called: ws.PageSetup.LeftMargin = 0;
[Test]
        public void Property_LeftMargin()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;NET45262/&quot;;

            string savePath = CreateFolder(filePath);
            Workbook wb = null;
            Worksheet ws = null;
            Style style = null;
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Borders = true;
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportActiveWorksheetOnly = true;
#region default
            wb = new Workbook(filePath + &quot;input.xlsx&quot;);
            ws = wb.Worksheets[0];
            wb.Worksheets.ActiveSheetIndex = 0;
            //render whole worksheet
            ws.PageSetup.BottomMargin = 0;
            ws.PageSetup.LeftMargin = 0;
            ws.PageSetup.RightMargin = 0;
            ws.PageSetup.TopMargin = 0;
            ws.PageSetup.PrintArea = string.Empty;

            options.HtmlCrossStringType = HtmlCrossType.Default;
            wb.Save(savePath + &quot;default_noBorder.html&quot;, options);

            wb = new Workbook(filePath + &quot;input.xlsx&quot;);
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
            wb.Save(savePath + &quot;default_border.html&quot;, options);
#endregion

#region cross
            wb = new Workbook(filePath + &quot;input.xlsx&quot;);
            ws = wb.Worksheets[0];
            wb.Worksheets.ActiveSheetIndex = 0;
            //render whole worksheet
            ws.PageSetup.BottomMargin = 0;
            ws.PageSetup.LeftMargin = 0;
            ws.PageSetup.RightMargin = 0;
            ws.PageSetup.TopMargin = 0;
            ws.PageSetup.PrintArea = string.Empty;

            options.HtmlCrossStringType = HtmlCrossType.Cross;
            wb.Save(savePath + &quot;cross_noBorder.html&quot;, options);

            wb = new Workbook(filePath + &quot;input.xlsx&quot;);
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
            wb.Save(savePath + &quot;cross_border.html&quot;, options);
#endregion

#region fitToCell
            wb = new Workbook(filePath + &quot;input-fit.xlsx&quot;);
            ws = wb.Worksheets[0];
            wb.Worksheets.ActiveSheetIndex = 0;
            //render whole worksheet
            ws.PageSetup.BottomMargin = 0;
            ws.PageSetup.LeftMargin = 0;
            ws.PageSetup.RightMargin = 0;
            ws.PageSetup.TopMargin = 0;
            ws.PageSetup.PrintArea = string.Empty;

            options.HtmlCrossStringType = HtmlCrossType.FitToCell;
            wb.Save(savePath + &quot;fitToCell_noBorder.html&quot;, options);

            wb = new Workbook(filePath + &quot;input-fit.xlsx&quot;);
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
            wb.Save(savePath + &quot;fitToCell_border.html&quot;, options);
#endregion

        }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


