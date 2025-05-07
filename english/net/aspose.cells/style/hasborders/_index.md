---
title: Style.HasBorders
second_title: Aspose.Cells for .NET API Reference
description: Style property. Checks whether there are borders have been set for the style
type: docs
url: /net/aspose.cells/style/hasborders/
---
## Style.HasBorders property

Checks whether there are borders have been set for the style.

```csharp
public bool HasBorders { get; }
```

### Examples

```csharp
// Called: Assert.IsTrue(style.HasBorders && style.Borders[BorderType.LeftBorder].Color == Color.FromArgb(0, 0, 0));
[Test]
        public void Property_HasBorders()
        {
            Workbook wb = new Workbook(Constants.HtmlPath + "CELLSNET-52761.html");
            Worksheet ws = wb.Worksheets[0];
            Style style = ws.Cells[5, 0].GetStyle();
            Assert.IsTrue(style.BackgroundColor == Color.FromArgb(0xFF, 0xB0, 0x62));
            Assert.IsTrue(style.HasBorders && style.Borders[BorderType.LeftBorder].Color == Color.FromArgb(0, 0, 0));
            wb.Save(_destFilesPath + "CELLSNET-52761.xlsx");
        }
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


