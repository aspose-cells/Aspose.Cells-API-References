---
title: "ChartArea.HeightRatioToChart"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ChartArea 属性。获取或设置其右下角行的垂直偏移量，单位为图表区域的比例"
type: docs
url: /zh/net/aspose.cells.charts/chartarea/heightratiotochart/
---
## ChartArea.HeightRatioToChart property

获取或设置右下角行的垂直偏移量，单位为图表区域的比例。

```csharp
public override double HeightRatioToChart { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartAreaPropertyHeightRatioToChartDemo
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

            // 访问图表区域
            ChartArea chartArea = chart.ChartArea;

            // 显示当前 HeightRatioToChart 值
            Console.WriteLine("Current HeightRatioToChart value: " + chartArea.HeightRatioToChart);

            // 为 HeightRatioToChart 设置新值（0.5 = 图表高度的 50%）
            chartArea.HeightRatioToChart = 0.5;
            Console.WriteLine("New HeightRatioToChart value: " + chartArea.HeightRatioToChart);

            // 为 WidthRatioToChart 设置新值以演示组合效果
            chartArea.WidthRatioToChart = 0.8;

            // 保存工作簿以查看更改
            workbook.Save("ChartAreaPropertyHeightRatioToChartDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


