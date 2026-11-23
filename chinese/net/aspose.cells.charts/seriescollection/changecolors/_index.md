---
title: "SeriesCollection.ChangeColors"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SeriesCollection 方法。为图表系列设置单色调调色板"
type: docs
url: /zh/net/aspose.cells.charts/seriescollection/changecolors/
---
## SeriesCollection.ChangeColors method

为图表系列设置单色调调色板。

```csharp
public void ChangeColors(ChartColorPaletteType type)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 类型 | ChartColorPaletteType | 单色调类型。 |

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionMethodChangeColorsWithChartColorPaletDemo
    {
        public static void Run()
        {
            // 创建新工作簿并获取第一个工作表
            Workbook workbook = new Workbook();
            Worksheet ws = workbook.Worksheets[0];

            // 为图表填充一些数据
            ws.Cells["A1"].PutValue("Category");
            ws.Cells["A2"].PutValue("Jan");
            ws.Cells["A3"].PutValue("Feb");
            ws.Cells["A4"].PutValue("Mar");

            ws.Cells["B1"].PutValue("Series1");
            ws.Cells["B2"].PutValue(10);
            ws.Cells["B3"].PutValue(20);
            ws.Cells["B4"].PutValue(30);

            ws.Cells["C1"].PutValue("Series2");
            ws.Cells["C2"].PutValue(15);
            ws.Cells["C3"].PutValue(25);
            ws.Cells["C4"].PutValue(35);

            // 添加柱形图
            int chartIdx = ws.Charts.Add(ChartType.Column, 6, 0, 20, 10);
            Chart chart = ws.Charts[chartIdx];

            // 设置系列的数据范围
            chart.NSeries.Add("B1:C4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // 获取系列集合
            SeriesCollection seriesColl = chart.NSeries;

            try
            {
                // 更改集合中所有系列的颜色调色板。
                // 使用数值强制转换为有效的枚举值（例如 0），以避免依赖的枚举成员名称。
                seriesColl.ChangeColors((ChartColorPaletteType)0);

                Console.WriteLine("ChangeColors method invoked successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error invoking ChangeColors: {ex.Message}");
            }

            // 保存工作簿以验证结果
            workbook.Save("SeriesCollection_ChangeColors_Demo.xlsx");
        }
    }
}
```

### 另请参见

* enum [ChartColorPaletteType](../../chartcolorpalettetype/)
* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


