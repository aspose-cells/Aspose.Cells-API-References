---
title: StyleFlag.TopBorder
second_title: Aspose.Cells for .NET API Reference
description: StyleFlag property. Top border settings will be applied
type: docs
url: /net/aspose.cells/styleflag/topborder/
---
## StyleFlag.TopBorder property

Top border settings will be applied.

```csharp
public bool TopBorder { get; set; }
```

### Examples

```csharp
// Called: styleFlag.TopBorder = true;
public void StyleFlag_Property_TopBorder()
{
    var myWorkbook = new Workbook(Constants.sourcePath + "example.xlsx");
    var mySheet = myWorkbook.Worksheets[myWorkbook.Worksheets.ActiveSheetIndex];
    //Create Style
    var style = myWorkbook.CreateStyle();
    style.VerticalAlignment = TextAlignmentType.Center;
    style.HorizontalAlignment = TextAlignmentType.Center;
    style.Font.Color = Color.Green;
    style.ShrinkToFit = true;

    //Setting the bottom border color of the cell to red
    style.Borders[BorderType.BottomBorder].Color = Color.Red;
    style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dotted;
    style.Borders[BorderType.TopBorder].Color = Color.Red;
    style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Dotted;
    //Creating StyleFlag
    var styleFlag = new StyleFlag();
    styleFlag.HorizontalAlignment = true;
    styleFlag.VerticalAlignment = true;
    styleFlag.ShrinkToFit = true;
    styleFlag.BottomBorder = true;
    styleFlag.TopBorder = true;
    styleFlag.FontColor = true;

    var row = mySheet.Cells.Rows[1];
    row.ApplyStyle(style, styleFlag);
    style = mySheet.Cells["A1"].GetStyle();
    Assert.AreEqual(style.Borders[BorderType.BottomBorder].LineStyle, CellBorderType.Dotted);
    style = mySheet.Cells["A3"].GetStyle();
    Assert.AreEqual(style.Borders[BorderType.TopBorder].LineStyle, CellBorderType.Dotted);
    //styleFlag.TopBorder = true;
    //row.ApplyStyle(style, styleFlag);
    myWorkbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


