---
title: "Chart.IsCellReferedByChart"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Chart 方法。返回图表是否引用了该单元格"
type: docs
url: /zh/net/aspose.cells.charts/chart/iscellreferedbychart/
---
## Chart.IsCellReferedByChart method

返回图表是否引用了该单元格。

```csharp
public bool IsCellReferedByChart(int sheetIndex, int rowIndex, int columnIndex)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sheetIndex | Int32 | 工作表索引 -1 表示包含当前图表的工作表。 |
| rowIndex | Int32 | 行索引 |
| columnIndex | Int32 | 列索引 |

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodIsCellReferedByChartWithInt32Int32Int32Demo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // 设置图表数据源
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // 检查单元格是否被图表引用
            bool isReferred = chart.IsCellReferedByChart(0, 1, 0); // Check if B2 is referred
            Console.WriteLine("Is cell B2 referred by chart: " + isReferred);
        }
    }
}
```

### 另请参见

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


