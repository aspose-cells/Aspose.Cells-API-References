---
title: "枚举 TickLabelAlignmentType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Charts.TickLabelAlignmentType 枚举。表示坐标轴刻度标签的文本对齐类型"
type: docs
url: /zh/net/aspose.cells.charts/ticklabelalignmenttype/
---
## TickLabelAlignmentType enumeration

表示坐标轴刻度标签的文本对齐类型

```csharp
public enum TickLabelAlignmentType
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Center | `0` | 指定文本居中。 |
| Left | `1` | 指定文本左对齐。 |
| Right | `2` | 指定文本右对齐。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TickLabelAlignmentTypeDemo
    {
        public static void TickLabelAlignmentTypeExample()
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

            // 向图表添加系列
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // 访问类别轴的刻度标签
            TickLabels tickLabels = chart.CategoryAxis.TickLabels;

            // 设置刻度标签的对齐类型
            tickLabels.AlignmentType = TickLabelAlignmentType.Center;

            // 保存工作簿
            workbook.Save("TickLabelAlignmentTypeExample.xlsx");

            return;
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


