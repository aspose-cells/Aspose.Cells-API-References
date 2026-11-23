---
title: "ChartArea.YRatioToChart"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ChartArea 属性。获取或获取其左上角行的垂直偏移量，单位为图表区域的比例"
type: docs
url: /zh/net/aspose.cells.charts/chartarea/yratiotochart/
---
## ChartArea.YRatioToChart property

获取或获取左上角行的垂直偏移量，单位为图表区域的比例。

```csharp
public override double YRatioToChart { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartAreaPropertyYRatioToChartDemo
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
            
            // 设置图表数据源
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // 访问图表区域
            ChartArea chartArea = chart.ChartArea;

            // 显示当前 YRatioToChart 值
            Console.WriteLine("Current YRatioToChart value: " + chartArea.YRatioToChart);

            // 更改 YRatioToChart 属性 (0.0 到 1.0 表示图表区域的 0% 到 100%)
            chartArea.YRatioToChart = 0.2; // Move chart area down by 20% of chart height

            // 显示新的 YRatioToChart 值
            Console.WriteLine("New YRatioToChart value: " + chartArea.YRatioToChart);

            // 保存工作簿以查看效果
            workbook.Save("ChartAreaPropertyYRatioToChartDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


