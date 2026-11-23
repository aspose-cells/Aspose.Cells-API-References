---
title: "ChartFrame.DefaultYRatioToChart"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ChartFrame 属性。表示默认位置的 y，单位为图表区域比例的分数"
type: docs
url: /zh/net/aspose.cells.charts/chartframe/defaultyratiotochart/
---
## ChartFrame.DefaultYRatioToChart property

表示默认位置的 y，单位为图表区域比例的分数。

```csharp
public double DefaultYRatioToChart { get; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultYRatioToChartDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 为图表添加示例数据
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            
            // 添加图表并获取其图表框架
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);
            
            // 获取图表框架（此情况下为标题）
            ChartFrame chartFrame = chart.Title;
            
            // 显示当前 DefaultYRatioToChart 值
            Console.WriteLine("Current DefaultYRatioToChart value: " + chartFrame.DefaultYRatioToChart);
            
            // 演示更改 YRatioToChart 如何影响位置（因为 DefaultYRatioToChart 为只读）
            Console.WriteLine("Current YRatioToChart value: " + chartFrame.YRatioToChart);
            chartFrame.YRatioToChart = 0.1; // Move title up
            Console.WriteLine("New YRatioToChart value: " + chartFrame.YRatioToChart);
            
            // 保存结果
            workbook.Save("PropertyDefaultYRatioToChartDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


