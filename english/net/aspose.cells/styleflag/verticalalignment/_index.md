---
title: StyleFlag.VerticalAlignment
second_title: Aspose.Cells for .NET API Reference
description: StyleFlag property. Vertical alignment setting will be applied
type: docs
url: /net/aspose.cells/styleflag/verticalalignment/
---
## StyleFlag.VerticalAlignment property

Vertical alignment setting will be applied.

```csharp
public bool VerticalAlignment { get; set; }
```

### Examples

```csharp
// Called: styleFlag.VerticalAlignment = true;
[Test]
        public void Property_VerticalAlignment()
        {

            Workbook myWorkbook = new Workbook(Constants.sourcePath + &quot;CellsNet45131.xlsx&quot;);
            var mySheet = myWorkbook.Worksheets[myWorkbook.Worksheets.ActiveSheetIndex];

            //Create Style 
            var style = myWorkbook.CreateStyle();
            style.VerticalAlignment = TextAlignmentType.Center;
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.Font.Color = Color.Green;
            style.ShrinkToFit = true;

            //Setting the bottom border color of the cell to red style.Borders[BorderType.BottomBorder].Color = Color.Red; 
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dotted;

            //Creating StyleFlag 
            var styleFlag = new StyleFlag();
            styleFlag.HorizontalAlignment = true;
            styleFlag.VerticalAlignment = true;
            styleFlag.ShrinkToFit = true;
            styleFlag.BottomBorder = true;
            //styleFlag.Borders = true; This statement instead of above one still does not produce expected results 
            styleFlag.FontColor = true;

            var row = mySheet.Cells.Rows[0];
            row.ApplyStyle(style, styleFlag);

            style = mySheet.Cells[&quot;L2&quot;].GetStyle();
            Assert.AreEqual(style.Borders[BorderType.LeftBorder].LineStyle, CellBorderType.Thin);
            myWorkbook.Save(Constants.destPath + &quot;CellsNet45131.xlsx&quot;);
        }
```

### See Also

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


