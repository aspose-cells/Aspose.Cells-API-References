---
title: "ChartCalculateOptions.ChartCalculateOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ChartCalculateOptions 构造函数。创建用于计算图表的选项"
type: docs
url: /zh/net/aspose.cells.charts/chartcalculateoptions/chartcalculateoptions/
---
## ChartCalculateOptions constructor

创建图表计算的选项。

```csharp
public ChartCalculateOptions()
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCalculateOptionsMethodCtorDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // 使用构造函数创建 ChartCalculateOptions
            ChartCalculateOptions calculateOptions = new ChartCalculateOptions();
            calculateOptions.UpdateAllPoints = true;
            
            // 使用选项重新计算图表
            chart.Calculate(calculateOptions);

            // 保存工作簿
            workbook.Save("ChartCalculateOptionsDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [ChartCalculateOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


