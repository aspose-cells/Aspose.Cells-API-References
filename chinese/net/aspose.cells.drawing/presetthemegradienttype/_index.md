---
title: "枚举 PresetThemeGradientType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Drawing.PresetThemeGradientType 枚举。表示预设主题渐变类型"
type: docs
url: /zh/net/aspose.cells.drawing/presetthemegradienttype/
---
## PresetThemeGradientType enumeration

表示预设主题渐变类型。

```csharp
public enum PresetThemeGradientType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| LightGradient | `0` | 浅色渐变 |
| TopSpotlight | `1` | 顶部聚光灯 |
| MediumGradient | `2` | 中等渐变 |
| BottomSpotlight | `3` | 底部聚光灯 |
| RadialGradient | `4` | 径向渐变 |

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DrawingClassPresetThemeGradientTypeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加示例数据
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Category 1");
            worksheet.Cells["A3"].PutValue("Category 2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // 添加图表
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B3", true);

            // 对第一系列应用渐变填充
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            series.Area.FillFormat.FillType = FillType.Gradient;
            series.Area.FillFormat.GradientFill.SetPresetThemeGradient(
                PresetThemeGradientType.RadialGradient, 
                ThemeColorType.Accent1);

            // 保存工作簿
            workbook.Save("PresetThemeGradientDemo.xlsx");
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


