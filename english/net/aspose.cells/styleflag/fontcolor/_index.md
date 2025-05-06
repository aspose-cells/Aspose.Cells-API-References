---
title: StyleFlag.FontColor
second_title: Aspose.Cells for .NET API Reference
description: StyleFlag property. Font color setting will be applied
type: docs
url: /net/aspose.cells/styleflag/fontcolor/
---
## StyleFlag.FontColor property

Font color setting will be applied.

```csharp
public bool FontColor { get; set; }
```

### Examples

```csharp
// Called: styleFlag.FontColor = true;
[Test]
        public void Property_FontColor()
        {
            Workbook wb = new Workbook(Constants.sourcePath +&quot;CellsNet23710.xls&quot;);
            Style newStyle = wb.CreateStyle();

            newStyle.Font.Color = System.Drawing.Color.Black;
            newStyle.BackgroundColor = System.Drawing.Color.White;
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.CellShading = true;
            styleFlag.FontColor = true;

            wb.Worksheets[0].Cells.ApplyStyle(newStyle, styleFlag);
            
            wb.Save(Constants.destPath + &quot;CellsNet23710.xls&quot;);
        }
```

### See Also

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


