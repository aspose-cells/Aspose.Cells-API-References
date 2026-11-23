---
title: "ChartFrame.XRatioToChart"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ChartFrame 属性。获取或设置以图表区域比例为单位的左上角的 x 坐标"
type: docs
url: /zh/net/aspose.cells.charts/chartframe/xratiotochart/
---
## ChartFrame.XRatioToChart property

获取或设置以图表区域比例为单位的左上角的 x 坐标。

```csharp
public virtual double XRatioToChart { get; set; }
```

### 备注

这是一个分数值，有效范围在 0-1 之间。如何将比例单位转换为像素？XPixel = XRatioToChart * Chart.ChartObject.Width;

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyXRatioToChartDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // 设置图表数据源
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // 访问作为 ChartFrame 的图表标题
            ChartFrame chartTitle = chart.Title;

            // 显示当前 XRatioToChart 值
            Console.WriteLine("Current XRatioToChart value: " + chartTitle.XRatioToChart);

            // 设置新的 XRatioToChart 值（0.5 表示从左侧起占图表宽度的 50%）
            chartTitle.XRatioToChart = 0.5;

            // 显示新位置
            Console.WriteLine("Title position after change - XRatioToChart: " + chartTitle.XRatioToChart);

            // 保存工作簿
            workbook.Save("ChartFrameXRatioToChartDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


