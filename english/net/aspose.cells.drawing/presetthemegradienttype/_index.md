---
title: Enum PresetThemeGradientType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Drawing.PresetThemeGradientType enum. Represents the preset theme gradient type
type: docs
url: /net/aspose.cells.drawing/presetthemegradienttype/
---
## PresetThemeGradientType enumeration

Represents the preset theme gradient type.

```csharp
public enum PresetThemeGradientType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| LightGradient | `0` | Light gradient |
| TopSpotlight | `1` | Top spotlight |
| MediumGradient | `2` | Medium gradient |
| BottomSpotlight | `3` | Bottom spotlight |
| RadialGradient | `4` | Radial gradient |

### Examples

```csharp
// Called: ser.Area.FillFormat.GradientFill.SetPresetThemeGradient(PresetThemeGradientType.RadialGradient, ThemeColorType.Accent1);
[Test]
        public void Type_PresetThemeGradientType()
        {
            var wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            sheet.Cells[&quot;A2&quot;].PutValue(&quot;カテゴリー1&quot;);
            sheet.Cells[&quot;A3&quot;].PutValue(&quot;カテゴリー2&quot;);
            sheet.Cells[&quot;A4&quot;].PutValue(&quot;カテゴリー3&quot;);
            sheet.Cells[&quot;B1&quot;].PutValue(&quot;列 1&quot;);
            sheet.Cells[&quot;B2&quot;].PutValue(4);
            sheet.Cells[&quot;B3&quot;].PutValue(20);
            sheet.Cells[&quot;B4&quot;].PutValue(50);
            sheet.Cells[&quot;C1&quot;].PutValue(&quot;列 2&quot;);
            sheet.Cells[&quot;C2&quot;].PutValue(50);
            sheet.Cells[&quot;C3&quot;].PutValue(100);
            sheet.Cells[&quot;C4&quot;].PutValue(150);

            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];

            chart.Title.Text = &quot;マーケット&quot;;
            chart.SetChartDataRange(&quot;A1:C4&quot;, true);
            Series ser = chart.NSeries[0];
            ser.Area.FillFormat.FillType = FillType.Gradient;
            ser.Area.FillFormat.GradientFill.SetPresetThemeGradient(PresetThemeGradientType.RadialGradient, ThemeColorType.Accent1);
            Assert.AreEqual(69, ser.Area.FillFormat.GradientFill.GradientStops[2].Position);

            wb.Save(Constants.destPath + &quot;CellsNet51925_1.xlsx&quot;);
        }
```

### See Also

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


