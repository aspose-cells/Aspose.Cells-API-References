---
title: GradientFill.SetPresetThemeGradient
second_title: Aspose.Cells for .NET API Reference
description: GradientFill method. Sets preset theme gradient fill
type: docs
url: /net/aspose.cells.drawing/gradientfill/setpresetthemegradient/
---
## GradientFill.SetPresetThemeGradient method

Sets preset theme gradient fill.

```csharp
public void SetPresetThemeGradient(PresetThemeGradientType gradientType, 
    ThemeColorType themeColorType)
```

| Parameter | Type | Description |
| --- | --- | --- |
| gradientType | PresetThemeGradientType | The preset gradient type. |
| themeColorType | ThemeColorType | The theme color type. |

### Examples

```csharp
// Called: ser.Area.FillFormat.GradientFill.SetPresetThemeGradient(PresetThemeGradientType.RadialGradient, ThemeColorType.Accent1);
public void GradientFill_Method_SetPresetThemeGradient()
{
    var wb = new Workbook();
    Worksheet sheet = wb.Worksheets[0];

    sheet.Cells["A2"].PutValue("カテゴリー1");
    sheet.Cells["A3"].PutValue("カテゴリー2");
    sheet.Cells["A4"].PutValue("カテゴリー3");
    sheet.Cells["B1"].PutValue("列 1");
    sheet.Cells["B2"].PutValue(4);
    sheet.Cells["B3"].PutValue(20);
    sheet.Cells["B4"].PutValue(50);
    sheet.Cells["C1"].PutValue("列 2");
    sheet.Cells["C2"].PutValue(50);
    sheet.Cells["C3"].PutValue(100);
    sheet.Cells["C4"].PutValue(150);

    int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
    Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];

    chart.Title.Text = "マーケット";
    chart.SetChartDataRange("A1:C4", true);
    Series ser = chart.NSeries[0];
    ser.Area.FillFormat.FillType = FillType.Gradient;
    ser.Area.FillFormat.GradientFill.SetPresetThemeGradient(PresetThemeGradientType.RadialGradient, ThemeColorType.Accent1);
    Assert.AreEqual(69, ser.Area.FillFormat.GradientFill.GradientStops[2].Position);

    wb.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* enum [PresetThemeGradientType](../../presetthemegradienttype/)
* enum [ThemeColorType](../../../aspose.cells/themecolortype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


