---
title: "ChartArea.XRatioToChart"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ChartArea 属性。获取或设置左上角列的水平偏移量，作为图表区域的比例"
type: docs
url: /zh/net/aspose.cells.charts/chartarea/xratiotochart/
---
## ChartArea.XRatioToChart property

获取或设置左上角列的水平偏移量，作为图表区域的比例。

```csharp
public override double XRatioToChart { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartAreaPropertyXRatioToChartDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 15, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // 获取图表区域
            ChartArea chartArea = chart.ChartArea;

            // 显示当前 XRatioToChart 值
            Console.WriteLine("Current XRatioToChart value: " + chartArea.XRatioToChart);

            // 更改 XRatioToChart 值以水平移动图表区域
            chartArea.XRatioToChart = 0.2; // 20% from the left of the chart container

            // 显示新的 XRatioToChart 值
            Console.WriteLine("New XRatioToChart value: " + chartArea.XRatioToChart);

            // 保存工作簿
            workbook.Save("ChartAreaXRatioToChartDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


