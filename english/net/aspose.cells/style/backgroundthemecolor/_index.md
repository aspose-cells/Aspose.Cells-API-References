---
title: Style.BackgroundThemeColor
second_title: Aspose.Cells for .NET API Reference
description: Style property. Gets and sets the background theme color
type: docs
url: /net/aspose.cells/style/backgroundthemecolor/
---
## Style.BackgroundThemeColor property

Gets and sets the background theme color.

```csharp
public ThemeColor BackgroundThemeColor { get; set; }
```

### Remarks

If the background color is not a theme color, NULL will be returned.

### Examples

```csharp
// Called: style.BackgroundThemeColor = c1;
public void Style_Property_BackgroundThemeColor()
{
    Workbook work = new Workbook();
    Cells cells = work.Worksheets[0].Cells;
    Style style = cells["A1"].GetStyle();
    style.Pattern = BackgroundType.Solid;
    style.ForegroundColor = Color.Red;
    Assert.AreEqual(Color.Red.ToArgb(), style.ForegroundArgbColor);
    style.Pattern = BackgroundType.Gray12;
    style.ForegroundColor = Color.Blue;
    style.BackgroundColor = Color.Yellow;

    Assert.AreEqual(Color.Blue.ToArgb(), style.ForegroundArgbColor);
    Assert.AreEqual(Color.Yellow.ToArgb(), style.BackgroundArgbColor);

    ThemeColor c0 = new ThemeColor(ThemeColorType.Accent6, 0.5);
    ThemeColor c1 = new ThemeColor(ThemeColorType.Accent2, 0.5);
    style.Pattern = BackgroundType.Gray12;
    style.ForegroundThemeColor = c0;
    style.BackgroundThemeColor = c1;

    Assert.AreEqual(ThemeColorType.Accent6, style.ForegroundThemeColor.ColorType);
    Assert.AreEqual(ThemeColorType.Accent2, style.BackgroundThemeColor.ColorType);
}
```

### See Also

* class [ThemeColor](../../themecolor/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


