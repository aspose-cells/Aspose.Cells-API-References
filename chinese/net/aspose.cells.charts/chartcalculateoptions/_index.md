---
title: "类 ChartCalculateOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Charts.ChartCalculateOptions 类。表示图表计算的选项"
type: docs
url: /zh/net/aspose.cells.charts/chartcalculateoptions/
---
## ChartCalculateOptions class

表示图表计算的选项。

```csharp
public class ChartCalculateOptions
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [ChartCalculateOptions](chartcalculateoptions/)() | 创建图表计算的选项。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [UpdateAllPoints](../../aspose.cells.charts/chartcalculateoptions/updateallpoints/) { get; set; } | 在执行图表计算时是否更新所有数据点。默认：False。当您希望专门获取图表中每个数据点的值时，请将其设为 true。如果此参数设为 True，计算图表时可能会生成新数据点。这可能会使 Excel 文件变大。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartCalculateOptionsDemo
    {
        public static void ChartCalculateOptionsExample()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 向工作表添加示例数据
            worksheet.Cells[0, 0].PutValue("Category");
            worksheet.Cells[0, 1].PutValue("Value");
            worksheet.Cells[1, 0].PutValue("A");
            worksheet.Cells[1, 1].PutValue(10);
            worksheet.Cells[2, 0].PutValue("B");
            worksheet.Cells[2, 1].PutValue(20);
            worksheet.Cells[3, 0].PutValue("C");
            worksheet.Cells[3, 1].PutValue(30);

            // 向工作表添加图表
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // 设置图表的数据范围
            chart.SetChartDataRange("A1:B4", true);

            // 创建 ChartCalculateOptions 的实例
            ChartCalculateOptions options = new ChartCalculateOptions
            {
                UpdateAllPoints = true // Set the property to update all data points
            };

            // 使用指定选项计算图表
            chart.Calculate(options);

            // 保存工作簿
            workbook.Save("ChartCalculateOptionsExample.xlsx");
            workbook.Save("ChartCalculateOptionsExample.pdf");
            return;
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


