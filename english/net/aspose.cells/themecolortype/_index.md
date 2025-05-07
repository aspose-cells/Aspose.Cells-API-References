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
// Called: series.DataLabels.Font.ThemeColor = new ThemeColor(ThemeColorType.Accent1, 10); // works
[Test]
        public void Type_ThemeColorType()
        {
            var workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[workbook.Worksheets.Add()];
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(1, 1, 2, 5);
            Chart chart = worksheet.Charts[worksheet.Charts.Add(ChartType.Line, 1, 1, 1, 1)];
            Series series = chart.NSeries[chart.NSeries.Add(range.RefersTo, true)];
            ThemeColor currentThemeColor = series.DataLabels.Font.ThemeColor; // null 
            series.DataLabels.Font.ThemeColor = new ThemeColor(ThemeColorType.Accent1, 10); // works 
            series.DataLabels.Font.ThemeColor = null; // Exception 
        }
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


