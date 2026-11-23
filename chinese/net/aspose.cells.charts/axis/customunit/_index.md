---
title: "Axis.CustomUnit"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Axis 属性。指定显示单位的自定义值"
type: docs
url: /zh/net/aspose.cells.charts/axis/customunit/
---
## Axis.CustomUnit property

指定显示单位的自定义值。

```csharp
[Obsolete("Use Axis.CustomDisplayUnit property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int CustomUnit { get; set; }
```

### 备注

注意：此属性已过时。请改用 Axis.CustomDisplayUnit 属性。此属性将在自 2025 年 2 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class AxisPropertyCustomUnitDemo
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
            worksheet.Cells["B2"].PutValue(1000000);
            worksheet.Cells["B3"].PutValue(2000000);
            worksheet.Cells["B4"].PutValue(3000000);

            // 添加柱形图
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // 设置图表数据源
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // 访问数值轴
                Axis valueAxis = chart.ValueAxis;

                // 将显示单位设置为自定义
                valueAxis.DisplayUnit = DisplayUnitType.Custom;

                // 设置自定义显示单位值
                valueAxis.CustomDisplayUnit = 1000000;

                // 显示 CustomUnit 属性值（已过时属性）
                Console.WriteLine("CustomUnit value: " + valueAxis.CustomUnit);

                // 保存工作簿
                workbook.Save("AxisPropertyCustomUnitDemo.xlsx");
                Console.WriteLine("CustomUnit has been demonstrated");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


