---
title: Font.ThemeColor
second_title: Aspose.Cells for .NET API Reference
description: Font property. Gets and sets the theme color
type: docs
url: /net/aspose.cells/font/themecolor/
---
## Font.ThemeColor property

Gets and sets the theme color.

```csharp
public ThemeColor ThemeColor { get; set; }
```

### Remarks

If the font color is not a theme color, NULL will be returned.

### Examples

```csharp
// Called: ThemeColor currentThemeColor = series.DataLabels.Font.ThemeColor; // null
[Test]
        public void Property_ThemeColor()
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

* class [ThemeColor](../../themecolor/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


