---
title: "SeriesCollection.SwapSeries"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SeriesCollection 方法。直接更改两个系列的顺序"
type: docs
url: /zh/net/aspose.cells.charts/seriescollection/swapseries/
---
## SeriesCollection.SwapSeries method

直接更改两个系列的顺序。

```csharp
public void SwapSeries(int sourceIndex, int destIndex)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceIndex | Int32 | 当前索引 |
| destIndex | Int32 | 目标索引 |

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionMethodSwapSeriesWithInt32Int32Demo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 为图表添加示例数据
            worksheet.Cells["A1"].PutValue("Series 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);
            
            worksheet.Cells["B1"].PutValue("Series 2");
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["B3"].PutValue(10);
            worksheet.Cells["B4"].PutValue(15);
            
            worksheet.Cells["C1"].PutValue("Series 3");
            worksheet.Cells["C2"].PutValue(8);
            worksheet.Cells["C3"].PutValue(16);
            worksheet.Cells["C4"].PutValue(24);

            // 添加图表
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // 设置图表数据范围
            chart.NSeries.Add("A1:C4", true);
            
            // 获取系列集合
            Aspose.Cells.Charts.SeriesCollection sc = chart.NSeries;
            
            // 打印原始系列名称
            Console.WriteLine("Original Series Order:");
            for (int i = 0; i < sc.Count; i++)
            {
                Console.WriteLine($"Series {i}: {sc[i].Name}");
            }
            
            // 交换系列 0 和 1
            sc.SwapSeries(0, 1);
            Console.WriteLine("\nAfter swapping series 0 and 1:");
            for (int i = 0; i < sc.Count; i++)
            {
                Console.WriteLine($"Series {i}: {sc[i].Name}");
            }
            
            // 交换系列 2 和 0
            sc.SwapSeries(2, 0);
            Console.WriteLine("\nAfter swapping series 2 and 0:");
            for (int i = 0; i < sc.Count; i++)
            {
                Console.WriteLine($"Series {i}: {sc[i].Name}");
            }
        }
    }
}
```

### 另请参见

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


