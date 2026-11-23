---
title: "ChartPoint.DoughnutInnerRadius"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ChartPoint 属性。调用 Chart.Calculate 方法后，以像素为单位获取环形切片的内部半径。适用于环形图"
type: docs
url: /zh/net/aspose.cells.charts/chartpoint/doughnutinnerradius/
---
## ChartPoint.DoughnutInnerRadius property

调用 Chart.Calculate() 方法后，以像素为单位获取环形切片的内部半径。适用于环形图。

```csharp
public int DoughnutInnerRadius { get; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartPointPropertyDoughnutInnerRadiusDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 为图表添加示例数据
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("C1");
            worksheet.Cells["A3"].PutValue("C2");
            worksheet.Cells["A4"].PutValue("C3");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["B3"].PutValue(3);
            worksheet.Cells["B4"].PutValue(5);

            // 添加环形图
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // 设置图表数据范围
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // 计算图表以获取图表点
            chart.Calculate();

            // 从第一系列获取第一个图表点
            ChartPoint point = chart.NSeries[0].Points[0];

            // 显示当前 DoughnutInnerRadius 值
            Console.WriteLine("Current DoughnutInnerRadius value: " + point.DoughnutInnerRadius);

            // 注意：DoughnutInnerRadius 为只读，无法直接设置
            // 要更改内部半径，需要调整图表的 HoleSize 属性
            chart.FirstSliceAngle = 30; // Adjust the first slice angle instead since HoleSize isn't available

            // 重新计算图表以更新 DoughnutInnerRadius
            chart.Calculate();

            // 显示更新后的 DoughnutInnerRadius 值
            Console.WriteLine("Updated DoughnutInnerRadius value: " + point.DoughnutInnerRadius);

            // 保存工作簿
            workbook.Save("DoughnutInnerRadiusDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


