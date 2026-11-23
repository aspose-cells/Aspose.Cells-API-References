---
title: "Title.YRatioToChart"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Title 属性。获取或设置左上角的 y 坐标，单位为图表区域的比例。像素中的 Y  YRatioToChart  Chart.ChartObject.Width"
type: docs
url: /zh/net/aspose.cells.charts/title/yratiotochart/
---
## Title.YRatioToChart property

获取或设置左上角的 y 坐标，单位为图表区域的比例。像素中的 Y = YRatioToChart * Chart.ChartObject.Width;

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

    public class TitlePropertyYRatioToChartDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // 设置图表数据源
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // 获取图表标题
            chart.Title.Text = "Sample Chart Title";
            Title chartTitle = chart.Title;

            // 显示当前 YRatioToChart 值
            Console.WriteLine("Current YRatioToChart value: " + chartTitle.YRatioToChart);

            // 更改 YRatioToChart 属性以垂直移动标题
            chartTitle.YRatioToChart = 0.1; // 10% from the top of the chart area
            Console.WriteLine("New YRatioToChart value: " + chartTitle.YRatioToChart);

            // 保存工作簿
            workbook.Save("TitlePropertyYRatioToChartDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


