---
title: "ChartFrame.Background"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ChartFrame 属性。获取和设置背景的显示模式。此属性仅在 Excel 2003 或更早版本中有效"
type: docs
url: /zh/net/aspose.cells.charts/chartframe/background/
---
## ChartFrame.Background property

获取和设置背景的显示模式。此属性仅在 Excel 2003 或更早版本中有效。

```csharp
[Obsolete("Use ChartFrame.Area.FillFormat.FillType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public BackgroundMode Background { get; set; }
```

### 备注

注意：此成员现已过时。请改用 ChartFrame.Area.FillFormat.FillType 属性。例如，如果需要将 BackgroundMode 设置为 Opaque，可以使用以下代码：Area.FillFormat.FillType = FillType.Solid; Area.FillFormat.SolidFill.Color = Color.Red; 此属性将在自 2012 年 1 月起的 12 个月后移除。Aspose 对给您带来的任何不便表示歉意。

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyBackgroundDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加示例数据
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // 添加图表
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // 配置图表数据
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // 配置带背景设置的数据标签
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            dataLabels.ShowValue = true;
            dataLabels.Background = BackgroundMode.Transparent;

            // 保存工作簿
            workbook.Save("ChartBackgroundDemo.xlsx");
        }
    }
}
```

### 另请参见

* enum [BackgroundMode](../../backgroundmode/)
* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


