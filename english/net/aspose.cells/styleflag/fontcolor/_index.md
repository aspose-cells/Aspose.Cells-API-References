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

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


