---
title: PageSetup.BottomMargin
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Represents the size of the bottom margin in unit of centimeters
type: docs
url: /net/aspose.cells/pagesetup/bottommargin/
---
## PageSetup.BottomMargin property

Represents the size of the bottom margin, in unit of centimeters.

```csharp
public double BottomMargin { get; set; }
```

### Examples

```csharp
// Called: ws.PageSetup.BottomMargin = 0;
[Test]
        public void Property_BottomMargin()
        {
            string filePath = Constants.JohnTest_PATH_SOURCE + @&quot;NET45299/&quot;;

            Workbook wb = new Workbook(filePath + &quot;Input.xlsx&quot;);
            Worksheet ws = wb.Worksheets[0];
            wb.Worksheets.ActiveSheetIndex = 0;
            //render whole worksheet
            ws.PageSetup.BottomMargin = 0;
            ws.PageSetup.LeftMargin = 0;
            ws.PageSetup.RightMargin = 0;
            ws.PageSetup.TopMargin = 0;
            ws.PageSetup.PrintArea = string.Empty;
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.HtmlCrossStringType = HtmlCrossType.FitToCell;
            wb.Save(CreateFolder(filePath) + &quot;fitToCell_noBorder.html&quot;, options);

            wb = new Workbook(filePath + &quot;Input.xlsx&quot;);
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
            Style style = wb.CreateStyle();
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Borders = true;
            ws.Cells.MaxDisplayRange.ApplyStyle(style, styleFlag);

            options.HtmlCrossStringType = HtmlCrossType.FitToCell;
            wb.Save(CreateFolder(filePath) + &quot;fitToCell_border.html&quot;, options);
        }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


