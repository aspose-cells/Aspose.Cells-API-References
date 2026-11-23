---
title: "Chart.PlotVisibleCellsOnly"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Chart 属性。指示是否仅绘制可见单元格"
type: docs
url: /zh/net/aspose.cells.charts/chart/plotvisiblecellsonly/
---
## Chart.PlotVisibleCellsOnly property

指示是否仅绘制可见单元格。

```csharp
public bool PlotVisibleCellsOnly { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyPlotVisibleCellsOnlyDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 添加示例数据
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);
            
            // 隐藏第 3 行
            worksheet.Cells.Rows[2].IsHidden = true;
            
            // 添加图表
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // 设置图表数据范围
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // 将 PlotVisibleCellsOnly 设置为 false（默认值为 true）
            chart.PlotVisibleCellsOnly = false;
            
            // 保存工作簿
            workbook.Save("ChartPlotVisibleCellsOnlyDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### 另请参见

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


