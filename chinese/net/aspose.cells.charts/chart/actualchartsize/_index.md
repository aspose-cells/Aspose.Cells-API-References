---
title: "Chart.ActualChartSize"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Chart 属性。获取图表的实际大小（单位为像素）"
type: docs
url: /zh/net/aspose.cells.charts/chart/actualchartsize/
---
## Chart.ActualChartSize property

获取图表的实际大小（单位为像素）。

```csharp
[Obsolete("Use Chart.GetActualSize() method instead.")]
public Size ActualChartSize { get; }
```

### 备注

注意：此成员已过时。请改用 Chart.GetActualSize() 方法。此属性将在自 2022 年 7 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPropertyActualChartSizeDemo
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

            // 添加图表
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // 计算图表以确保属性已填充
            chart.Calculate();

            // 演示 ActualChartSize 的用法
            Console.WriteLine($"Actual Chart Size - Width: {chart.ActualChartSize.Width}, Height: {chart.ActualChartSize.Height}");

            // 添加一个大小基于 ActualChartSize 的形状
            Shape shape = chart.Shapes.AddShapeInChartByScale(
                MsoDrawingType.Rectangle,
                PlacementType.Move,
                0.5,  // x position (relative)
                0.5,  // y position (relative)
                0.5 + (0.1 * chart.ActualChartSize.Height / chart.ActualChartSize.Width),  // width adjusted by aspect ratio
                0.6   // height
            );
            shape.Fill.SolidFill.Color = Color.Blue;

            // 保存工作簿
            workbook.Save("ChartWithActualSizeDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


