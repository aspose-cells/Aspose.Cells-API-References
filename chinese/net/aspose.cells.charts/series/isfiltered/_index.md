---
title: "Series.IsFiltered"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Series 属性。指示系列是否被选中或过滤。True 表示此系列已被过滤，且不会在图表上显示"
type: docs
url: /zh/net/aspose.cells.charts/series/isfiltered/
---
## Series.IsFiltered property

指示系列是否被选中或过滤。True 表示此系列已被过滤，且不会在图表上显示。

```csharp
public bool IsFiltered { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyIsFilteredDemo
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
            worksheet.Cells["A5"].PutValue("D");
            
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);
            
            worksheet.Cells["C1"].PutValue("Series2");
            worksheet.Cells["C2"].PutValue(15);
            worksheet.Cells["C3"].PutValue(25);
            worksheet.Cells["C4"].PutValue(35);
            worksheet.Cells["C5"].PutValue(45);
            
            // 添加图表
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // 设置图表数据范围
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.Add("C2:C5", true);
            chart.NSeries.CategoryData = "A2:A5";
            
            // 演示 IsFiltered 属性
            Console.WriteLine("Initial Series Count: " + chart.NSeries.Count);
            
            // 过滤第一系列
            chart.NSeries[0].IsFiltered = true;
            Console.WriteLine("After filtering first series: " + chart.NSeries.Count);
            
            // 过滤第二系列
            chart.NSeries[0].IsFiltered = true;
            Console.WriteLine("After filtering second series: " + chart.NSeries.Count);
            
            // 保存工作簿
            workbook.Save("SeriesFilteredDemo_out.xlsx");
        }
    }
}
```

### 另请参见

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


