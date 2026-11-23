---
title: "枚举 ChartColorPaletteType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Charts.ChartColorPaletteType 枚举。枚举 Excel 图表中使用的所有单色调色板"
type: docs
url: /zh/net/aspose.cells.charts/chartcolorpalettetype/
---
## ChartColorPaletteType enumeration

枚举 Excel 图表中使用的所有单色调色板。

```csharp
public enum ChartColorPaletteType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| MonochromaticPalette1 | `1` | accent1 主题颜色渐变，深到浅。 |
| MonochromaticPalette2 | `2` | accent2 主题颜色渐变，深到浅。 |
| MonochromaticPalette3 | `3` | accent3 主题颜色渐变，深到浅。 |
| MonochromaticPalette4 | `4` | accent4 主题颜色渐变，深到浅。 |
| MonochromaticPalette5 | `5` | accent5 主题颜色渐变，深到浅。 |
| MonochromaticPalette6 | `6` | accent6 主题颜色渐变，深到浅。 |
| MonochromaticPalette7 | `7` | accent7 主题颜色渐变。 |
| MonochromaticPalette8 | `8` | accent1 主题颜色渐变，浅到深。 |
| MonochromaticPalette9 | `9` | accent2 主题颜色渐变，浅到深。 |
| MonochromaticPalette10 | `10` | accent3 主题颜色渐变，浅到深。 |
| MonochromaticPalette11 | `11` | accent4 主题颜色渐变，浅到深。 |
| MonochromaticPalette12 | `12` | accent5 主题颜色渐变，浅到深。 |
| MonochromaticPalette13 | `13` | accent6 主题颜色渐变，从浅到深。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartsClassChartColorPaletteTypeDemo
    {
        public static void Run()
        {
            // 创建一个用于演示的新工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // 添加示例图表以演示颜色调色板
                int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);
                Chart chart = worksheet.Charts[chartIndex];

                // 演示使用不同的 ChartColorPaletteType 枚举值
                ChartColorPaletteType palette1 = ChartColorPaletteType.MonochromaticPalette1;
                ChartColorPaletteType palette5 = ChartColorPaletteType.MonochromaticPalette5;
                ChartColorPaletteType palette8 = ChartColorPaletteType.MonochromaticPalette8;

                // 显示枚举值
                Console.WriteLine($"MonochromaticPalette1 value: {(int)palette1}");
                Console.WriteLine($"MonochromaticPalette5 value: {(int)palette5}");
                Console.WriteLine($"MonochromaticPalette8 value: {(int)palette8}");

                // 保存工作簿
                workbook.Save("ChartColorPaletteTypeDemo.xlsx");
                Console.WriteLine("ChartColorPaletteType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ChartColorPaletteType: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


