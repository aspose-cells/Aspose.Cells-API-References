---
title: Enum ThemeColorType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.ThemeColorType enum. Enumerates the theme color types
type: docs
url: /net/aspose.cells/themecolortype/
---
## ThemeColorType enumeration

Enumerates the theme color types.

```csharp
public enum ThemeColorType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Background1 | `0` |  |
| Text1 | `1` |  |
| Background2 | `2` |  |
| Text2 | `3` |  |
| Accent1 | `4` |  |
| Accent2 | `5` |  |
| Accent3 | `6` |  |
| Accent4 | `7` |  |
| Accent5 | `8` |  |
| Accent6 | `9` |  |
| Hyperlink | `10` |  |
| FollowedHyperlink | `11` |  |
| StyleColor | `12` | Inner used. A color used in theme definitions which means to use the color of the style. |

### Examples

```csharp
// Called: Assert.AreEqual(ThemeColorType.Accent6, style.ForegroundThemeColor.ColorType);
public void Cells_Type_ThemeColorType()
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

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


