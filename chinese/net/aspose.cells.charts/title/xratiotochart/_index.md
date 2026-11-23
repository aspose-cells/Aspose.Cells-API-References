---
title: "Title.XRatioToChart"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Title 属性。获取或设置左上角的 x 坐标，单位为图表区域的比例。像素中的 X  XRatioToChart  Chart.ChartObject.Width"
type: docs
url: /zh/net/aspose.cells.charts/title/xratiotochart/
---
## Title.XRatioToChart property

获取或设置左上角的 x 坐标，单位为图表区域的比例。像素中的 X = XRatioToChart * Chart.ChartObject.Width;

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

    public class TitlePropertyXRatioToChartDemo
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

            // 设置图表的数据源
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // 获取图表标题
            chart.Title.Text = "Sample Chart Title";
            Title title = chart.Title;

            // 显示当前 XRatioToChart 值
            Console.WriteLine("Current XRatioToChart value: " + title.XRatioToChart);

            // 更改 XRatioToChart 值以水平移动标题
            title.XRatioToChart = 0.25; // 25% from the left of the chart area
            Console.WriteLine("New XRatioToChart value: " + title.XRatioToChart);

            // 保存工作簿
            workbook.Save("TitlePropertyXRatioToChartDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


