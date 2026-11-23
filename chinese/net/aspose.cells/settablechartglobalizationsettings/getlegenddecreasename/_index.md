---
title: "SettableChartGlobalizationSettings.GetLegendDecreaseName"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SettableChartGlobalizationSettings 方法。获取图例中“减少”的名称"
type: docs
url: /zh/net/aspose.cells/settablechartglobalizationsettings/getlegenddecreasename/
---
## SettableChartGlobalizationSettings.GetLegendDecreaseName method

获取图例递减的名称。

```csharp
public override string GetLegendDecreaseName()
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetLegendDecreaseNameDemo
    {
        public static void Run()
        {
            // 创建新工作簿并获取第一个工作表
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加简单数据以提供上下文（可选）
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            // 创建图表（可选，仅用于完整的工作簿）
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // 实例化全局化设置对象
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // 设置自定义图例减少标签
                settings.SetLegendDecreaseName("Custom Decrease Label");

                // 使用 GetLegendDecreaseName 检索标签
                string legendDecreaseName = settings.GetLegendDecreaseName();

                Console.WriteLine("Legend Decrease Name: " + legendDecreaseName);

                // 保存工作簿（在此演示中，设置未直接附加到图表）
                workbook.Save("GetLegendDecreaseNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetLegendDecreaseName: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


