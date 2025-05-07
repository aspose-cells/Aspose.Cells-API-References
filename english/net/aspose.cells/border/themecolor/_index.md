---
title: Border.ThemeColor
second_title: Aspose.Cells for .NET API Reference
description: Border property. Gets and sets the theme color of the border
type: docs
url: /net/aspose.cells/border/themecolor/
---
## Border.ThemeColor property

Gets and sets the theme color of the border.

```csharp
public ThemeColor ThemeColor { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(style.Borders[BorderType.BottomBorder].ThemeColor.ColorType, ThemeColorType.Accent1);
[Test]
        public void Property_ThemeColor()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSJAVA41198.xlsx");
            Style style = workbook.Worksheets[0].Cells["F1"].GetStyle();
            Assert.AreEqual(style.Borders[BorderType.BottomBorder].ThemeColor.ColorType, ThemeColorType.Accent1);
        }
```

### See Also

* class [ThemeColor](../../themecolor/)
* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


