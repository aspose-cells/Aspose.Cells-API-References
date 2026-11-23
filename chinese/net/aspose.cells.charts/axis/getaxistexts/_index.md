---
title: "Axis.GetAxisTexts"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Axis 方法。调用 Chart.Calculate 方法后获取坐标轴的标签"
type: docs
url: /zh/net/aspose.cells.charts/axis/getaxistexts/
---
## Axis.GetAxisTexts method

调用 Chart.Calculate() 方法后获取坐标轴的标签。

```csharp
public string[] GetAxisTexts()
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisMethodGetAxisTextsDemo
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
            worksheet.Cells["B2"].PutValue(8000);
            worksheet.Cells["B3"].PutValue(4000);
            worksheet.Cells["B4"].PutValue(-8000);

            // 添加图表
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // 设置图表数据范围
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // 计算图表
            chart.Calculate();
            
            // 获取坐标轴标签
            string[] labels = chart.ValueAxis.GetAxisTexts();
            
            // 输出标签
            Console.WriteLine("Value Axis Labels:");
            foreach (string label in labels)
            {
                Console.WriteLine(label);
            }
        }
    }
}
```

### 另请参见

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


