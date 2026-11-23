---
title: "ChartFrame.YRatioToChart"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ChartFrame 属性。获取或设置左上角的 y 坐标，单位为图表区域比例"
type: docs
url: /zh/net/aspose.cells.charts/chartframe/yratiotochart/
---
## ChartFrame.YRatioToChart property

获取或设置左上角的 y 坐标，单位为图表区域比例。

```csharp
public virtual double YRatioToChart { get; set; }
```

### 备注

这是一个分数值，有效范围在 0-1 之间。如何将比例单位转换为像素？YPixel = YRatioToChart * Chart.ChartObject.Height;

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyYRatioToChartDemo
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
            
            // 访问继承自 ChartFrame 的图表标题
            chart.Title.Text = "Sample Chart";
            
            // 显示当前 YRatioToChart 值
            Console.WriteLine("Current Title YRatioToChart value: " + chart.Title.YRatioToChart);
            
            // 更改标题相对于图表区域的 Y 位置
            chart.Title.YRatioToChart = 0.1; // 10% from top of chart area
            
            // 显示新的 YRatioToChart 值
            Console.WriteLine("New Title YRatioToChart value: " + chart.Title.YRatioToChart);
            
            // 访问同样继承自 ChartFrame 的图例
            chart.Legend.Position = LegendPositionType.Top;
            
            // 显示图例当前的 YRatioToChart 值
            Console.WriteLine("Current Legend YRatioToChart value: " + chart.Legend.YRatioToChart);
            
            // 更改图例相对于图表区域的 Y 位置
            chart.Legend.YRatioToChart = 0.15; // 15% from top of chart area
            
            // 显示图例新的 YRatioToChart 值
            Console.WriteLine("New Legend YRatioToChart value: " + chart.Legend.YRatioToChart);
            
            // 保存工作簿
            workbook.Save("ChartFramePropertyYRatioToChartDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


