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
// Called: style.Font.ThemeColor = new ThemeColor(ThemeColorType.Text2, 0.4);
public static void Type_ThemeColorType()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Adding a value to cell A1
            cells[&quot;A1&quot;].PutValue(&quot;Hello World&quot;);

            // Getting the style of cell A1
            Style style = cells[&quot;A1&quot;].GetStyle();

            // Set ThemeColorType.Text2 color type with 40% lighten as the font color.
            style.Font.ThemeColor = new ThemeColor(ThemeColorType.Text2, 0.4);
            style.Pattern = BackgroundType.Solid;

            // Set ThemeColorType.Background2 color type with 75% darken as the foreground color
            style.ForegroundThemeColor = new ThemeColor(ThemeColorType.Background2, -0.75);

            // Applying the style to cell A1
            cells[&quot;A1&quot;].SetStyle(style);

            // Saving the Excel file
            workbook.Save(&quot;ThemeColorExample.xlsx&quot;);
        }
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


