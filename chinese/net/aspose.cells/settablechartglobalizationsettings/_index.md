---
title: "类 SettableChartGlobalizationSettings"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.SettableChartGlobalizationSettings 类。实现 PivotGlobalizationSettings，支持用户设置/更改预定义文本"
type: docs
url: /zh/net/aspose.cells/settablechartglobalizationsettings/
---
## SettableChartGlobalizationSettings class

实现 PivotGlobalizationSettings，支持用户设置/更改预定义文本。

```csharp
public class SettableChartGlobalizationSettings : ChartGlobalizationSettings
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [SettableChartGlobalizationSettings](settablechartglobalizationsettings/)() | 默认构造函数。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| override [GetAxisTitleName](../../aspose.cells/settablechartglobalizationsettings/getaxistitlename/)() | 获取轴标题的名称。 |
| override [GetAxisUnitName](../../aspose.cells/settablechartglobalizationsettings/getaxisunitname/)(DisplayUnitType) | 获取轴单位的名称。 |
| override [GetChartTitleName](../../aspose.cells/settablechartglobalizationsettings/getcharttitlename/)() | 获取图表标题的名称。 |
| override [GetLegendDecreaseName](../../aspose.cells/settablechartglobalizationsettings/getlegenddecreasename/)() | 获取图例递减的名称。 |
| override [GetLegendIncreaseName](../../aspose.cells/settablechartglobalizationsettings/getlegendincreasename/)() | 获取图例的增加名称。 |
| override [GetLegendTotalName](../../aspose.cells/settablechartglobalizationsettings/getlegendtotalname/)() | 获取图例的总计名称。 |
| override [GetOtherName](../../aspose.cells/settablechartglobalizationsettings/getothername/)() | 获取图表的 "Other" 标签名称。 |
| override [GetSeriesName](../../aspose.cells/settablechartglobalizationsettings/getseriesname/)() | 获取图表中系列的名称。 |
| [SetAxisTitleName](../../aspose.cells/settablechartglobalizationsettings/setaxistitlename/)(string) | 设置轴的标题名称。 |
| [SetAxisUnitName](../../aspose.cells/settablechartglobalizationsettings/setaxisunitname/)(DisplayUnitType, string) | 设置轴单位的名称。 |
| [SetChartTitleName](../../aspose.cells/settablechartglobalizationsettings/setcharttitlename/)(string) | 设置图表标题的名称。 |
| [SetLegendDecreaseName](../../aspose.cells/settablechartglobalizationsettings/setlegenddecreasename/)(string) | 设置图例的减少名称。 |
| [SetLegendIncreaseName](../../aspose.cells/settablechartglobalizationsettings/setlegendincreasename/)(string) | 设置图例的增加名称。 |
| [SetLegendTotalName](../../aspose.cells/settablechartglobalizationsettings/setlegendtotalname/)(string) | 设置图例的总计名称。 |
| [SetOtherName](../../aspose.cells/settablechartglobalizationsettings/setothername/)(string) | 设置图表的 "Other" 标签名称。 |
| [SetSeriesName](../../aspose.cells/settablechartglobalizationsettings/setseriesname/)(string) | 设置图表中系列的名称。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class CellsClassSettableChartGlobalizationSettingsDemo
    {
        public static void Run()
        {
            // 创建一个用于演示的新工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // 创建 SettableChartGlobalizationSettings 的实例
                var settings = new SettableChartGlobalizationSettings();

                // 设置自定义全局化设置
                settings.SetSeriesName("Custom Series");
                settings.SetChartTitleName("Custom Chart Title");
                settings.SetLegendIncreaseName("Custom Increase");
                settings.SetLegendDecreaseName("Custom Decrease");

                // 创建自定义 GlobalizationSettings 实现
                workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings(settings);

                // 创建一个简单的图表来演示这些设置
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["A2"].PutValue("Q1");
                worksheet.Cells["A3"].PutValue("Q2");
                worksheet.Cells["B1"].PutValue("Value");
                worksheet.Cells["B2"].PutValue(100);
                worksheet.Cells["B3"].PutValue(200);

                int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
                Chart chart = worksheet.Charts[chartIndex];
                chart.NSeries.Add("B2:B3", true);
                chart.NSeries.CategoryData = "A2:A3";
                chart.Title.Text = "Demo Chart";

                Console.WriteLine("SettableChartGlobalizationSettings configured successfully");
                workbook.Save("SettableChartGlobalizationSettingsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SettableChartGlobalizationSettings: {ex.Message}");
            }
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            private readonly SettableChartGlobalizationSettings _chartSettings;

            public CustomGlobalizationSettings(SettableChartGlobalizationSettings chartSettings)
            {
                _chartSettings = chartSettings;
            }

            // 在此实现所需的 GlobalizationSettings 方法
            // 该委托给 SettableChartGlobalizationSettings 实例
        }
    }
}
```

### 另请参见

* class [ChartGlobalizationSettings](../../aspose.cells.charts/chartglobalizationsettings/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


