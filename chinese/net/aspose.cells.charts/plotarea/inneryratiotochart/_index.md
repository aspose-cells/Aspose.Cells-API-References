---
title: "PlotArea.InnerYRatioToChart"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PlotArea 属性。获取或获取绘图区左上角的 x 坐标，单位为图表区域比例"
type: docs
url: /zh/net/aspose.cells.charts/plotarea/inneryratiotochart/
---
## PlotArea.InnerYRatioToChart property

获取或获取绘图区左上角的 x 坐标，单位为图表区域比例。

```csharp
public double InnerYRatioToChart { get; set; }
```

### 备注

绘图区的边界框包括绘图区、刻度线（刻度标签）以及刻度线周围的一小段边框。如果该值不是由 MS Excel 创建的，请在调用此方法之前调用 Chart.Calculate() 方法。

**PlotArea** 的 **XRatioToChart**, **YRatioToChart**, **WidthRatioToChart** 和 **HeightRatioToChart** 表示包含绘图区、刻度线（刻度标签）以及刻度线周围小边框的绘图区边界框。如果想获取绘图区的实际尺寸，应调用 **InnerXRatioToChart**、**InnerYRatioToChart**、**InnerWidthRatioToChart** 和 **InnerHeightRatioToChart** 属性。

对于 Excel 2007 或更高版本，默认值为零。应在调用 Chart.Calculate() 之后获取该值。

像素中的 InnerY = InnerYRatioToChart * chart.ChartObject.Width。注意：当设置 InnerYRatioToChart 时，IsInnerMode 属性将自动设置为 True。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PlotAreaPropertyInnerYRatioToChartDemo
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

            // 获取图表的绘图区
            PlotArea plotArea = chart.PlotArea;

            // 显示当前 InnerYRatioToChart 值
            Console.WriteLine("Current InnerYRatioToChart value: " + plotArea.InnerYRatioToChart);

            // 更改 InnerYRatioToChart 值（0.0 到 1.0 表示图表区域的 0% 到 100%）
            plotArea.InnerYRatioToChart = 0.2;

            // 显示新值
            Console.WriteLine("New InnerYRatioToChart value: " + plotArea.InnerYRatioToChart);

            // 保存工作簿
            workbook.Save("PlotAreaPropertyInnerYRatioToChartDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [PlotArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


