---
title: "TickLabels.TextDirection"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "TickLabels 属性。表示文本阅读顺序"
type: docs
url: /zh/net/aspose.cells.charts/ticklabels/textdirection/
---
## TickLabels.TextDirection property

表示文本阅读顺序。

```csharp
[Obsolete("Use TickLabels.ReadingOrder property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public TextDirectionType TextDirection { get; set; }
```

### 备注

注意：此成员已过时。请改用 TickLabels.ReadingOrder 属性。此属性将在自 2020 年 3 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyTextDirectionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加示例数据
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // 添加图表
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // 配置刻度标签文本方向
            Axis valueAxis = chart.ValueAxis;
            TickLabels tickLabels = valueAxis.TickLabels;
            tickLabels.TextDirection = TextDirectionType.LeftToRight;

            workbook.Save("TickLabelsTextDirectionDemo.xlsx");
        }
    }
}
```

### 另请参见

* enum [TextDirectionType](../../../aspose.cells/textdirectiontype/)
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


