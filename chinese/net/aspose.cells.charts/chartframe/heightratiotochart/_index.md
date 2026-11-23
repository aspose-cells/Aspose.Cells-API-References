---
title: "ChartFrame.HeightRatioToChart"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ChartFrame 属性。获取或设置以图表区域比例为单位的框高度"
type: docs
url: /zh/net/aspose.cells.charts/chartframe/heightratiotochart/
---
## ChartFrame.HeightRatioToChart property

获取或设置以图表区域比例为单位的框高度。

```csharp
public virtual double HeightRatioToChart { get; set; }
```

### 备注

这是一个分数值，有效范围在 0-1 之间。如何将比例单位转换为像素？HeightPixel = HeightRatioToChart * Chart.ChartObject.Height;

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyHeightRatioToChartDemo
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

            // 向工作表添加图表
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // 设置图表数据源
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // 访问图表标题（继承自 ChartFrame）
            chart.Title.Text = "Sample Chart";
            ChartFrame titleFrame = chart.Title;

            // 显示当前 HeightRatioToChart 值
            Console.WriteLine("Current HeightRatioToChart value: " + titleFrame.HeightRatioToChart);

            // 设置新的高度比例（0.1 = 图表高度的 10%）
            titleFrame.HeightRatioToChart = 0.1;

            // 通过前后对比演示效果
            Console.WriteLine("Title height reduced to 10% of chart height");

            // 保存结果
            workbook.Save("PropertyHeightRatioToChartDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


