---
title: Style.BackgroundColor
second_title: Aspose.Cells for .NET API Reference
description: Style property. Gets or sets a styles background color
type: docs
url: /net/aspose.cells/style/backgroundcolor/
---
## Style.BackgroundColor property

Gets or sets a style's background color.

```csharp
public Color BackgroundColor { get; set; }
```

### Remarks

If you want to set a cell's color, please use Style.ForegroundColor property. Only if the cell style pattern is other than none or solid, this property will take effect.

### Examples

```csharp
// Called: cellStyle.BackgroundColor = System.Drawing.Color.Empty;
public void Style_Property_BackgroundColor()
{
    Workbook wb = new Workbook(Constants.sourcePath + "testfile_new.xls");
    StyleFlag styleFlag = new StyleFlag();
    Style cellStyle = null;

          

    cellStyle = wb.CreateStyle();

    cellStyle.Font.Color = System.Drawing.Color.Black;
    cellStyle.BackgroundColor = System.Drawing.Color.Empty;
    cellStyle.ForegroundColor = System.Drawing.Color.Empty;
    cellStyle.Pattern = BackgroundType.None;
    styleFlag.FontColor = true;
    styleFlag.CellShading = true;
    for (int i = 0; i < wb.Worksheets.Count; i++)
    {
        Cells allCells = wb.Worksheets[i].Cells;
        allCells.ApplyStyle(cellStyle, styleFlag);
    }
            

    wb.Save(Constants.destPath + "testfile_new.xls");
            
}
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


