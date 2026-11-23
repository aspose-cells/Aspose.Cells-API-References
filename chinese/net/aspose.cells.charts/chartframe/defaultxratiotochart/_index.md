---
title: "ChartFrame.DefaultXRatioToChart"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ChartFrame 属性。表示默认位置的 x，单位为图表区域的比例分数"
type: docs
url: /zh/net/aspose.cells.charts/chartframe/defaultxratiotochart/
---
## ChartFrame.DefaultXRatioToChart property

表示默认位置的 x，单位为图表区域的比例分数。

```csharp
public double DefaultXRatioToChart { get; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyDefaultXRatioToChartDemo
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

            // 获取图表标题框架
            ChartFrame titleFrame = chart.Title;

            // 显示当前 DefaultXRatioToChart 值
            Console.WriteLine("Default X Ratio To Chart (Title): " + titleFrame.DefaultXRatioToChart);

            // 在图表中创建文本框
            Aspose.Cells.Drawing.TextBox textBox = chart.Shapes.AddTextBoxInChart(50, 50, 200, 100);
            
            // 获取文本框的形状属性，而不是尝试直接访问 ChartFrame
            Console.WriteLine("Default X Ratio To Chart (TextBox): " + titleFrame.DefaultXRatioToChart);

            // 演示这些默认比例如何影响定位
            Console.WriteLine("Title X Position (Ratio): " + titleFrame.XRatioToChart);
            Console.WriteLine("TextBox X Position (Ratio): " + titleFrame.XRatioToChart);

            // 保存工作簿
            workbook.Save("ChartFrameDefaultXRatioToChartDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


