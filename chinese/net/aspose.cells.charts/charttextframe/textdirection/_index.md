---
title: "ChartTextFrame.TextDirection"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ChartTextFrame 属性。表示文本阅读顺序"
type: docs
url: /zh/net/aspose.cells.charts/charttextframe/textdirection/
---
## ChartTextFrame.TextDirection property

表示文本阅读顺序。

```csharp
[Obsolete("Use ChartTextFrame.ReadingOrder property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public TextDirectionType TextDirection { get; set; }
```

### 备注

注意：此成员已过时。请改用 ChartTextFrame.ReadingOrder 属性。该属性将在自 2020 年 3 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyTextDirectionDemo
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

            // 配置数据标签
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            dataLabels.ShowValue = true;
            
            // 演示 TextDirection 属性
            dataLabels.TextDirection = TextDirectionType.LeftToRight;

            // 保存工作簿
            workbook.Save("ChartTextDirectionDemo.xlsx");
        }
    }
}
```

### 另请参见

* enum [TextDirectionType](../../../aspose.cells/textdirectiontype/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


