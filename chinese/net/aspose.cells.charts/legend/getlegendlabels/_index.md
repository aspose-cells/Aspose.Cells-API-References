---
title: "Legend.GetLegendLabels"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Legend 方法。调用 Chart.Calculate 方法后获取图例项的标签"
type: docs
url: /zh/net/aspose.cells.charts/legend/getlegendlabels/
---
## Legend.GetLegendLabels method

在调用 Chart.Calculate() 方法后获取图例项的标签。

```csharp
public string[] GetLegendLabels()
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LegendMethodGetLegendLabelsDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 访问第一个工作表
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // 设置图表数据范围
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // 计算图表
            chart.Calculate();
            
            // 获取图例标签
            string[] legendLabels = chart.Legend.GetLegendLabels();
            
            // 显示图例标签
            Console.WriteLine("Legend Labels:");
            foreach (string label in legendLabels)
            {
                Console.WriteLine(label);
            }
        }
    }
}
```

### 另请参见

* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


