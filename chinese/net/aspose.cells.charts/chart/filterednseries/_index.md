---
title: "Chart.FilteredNSeries"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Chart 属性。获取表示在图表中被过滤的数据系列的 SeriesCollection 集合"
type: docs
url: /zh/net/aspose.cells.charts/chart/filterednseries/
---
## Chart.FilteredNSeries property

获取表示在图表中被过滤的数据系列的 [`SeriesCollection`](../../seriescollection/) 集合。

```csharp
public SeriesCollection FilteredNSeries { get; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyFilteredNSeriesDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 为图表添加示例数据
            worksheet.Cells["A1"].PutValue("Series");
            worksheet.Cells["A2"].PutValue("Series 1");
            worksheet.Cells["A3"].PutValue("Series 2");
            worksheet.Cells["A4"].PutValue("Series 3");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // 添加图表并将某些系列设为过滤状态
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // 过滤某些系列（隐藏系列 2）
            chart.NSeries[1].IsFiltered = true;

            // 访问过滤后的系列集合
            Aspose.Cells.Charts.SeriesCollection filteredSeries = chart.FilteredNSeries;
            Console.WriteLine("Filtered Series Count: " + filteredSeries.Count.ToString());

            // 保存工作簿
            workbook.Save("FilteredNSeriesDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [SeriesCollection](../../seriescollection/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


