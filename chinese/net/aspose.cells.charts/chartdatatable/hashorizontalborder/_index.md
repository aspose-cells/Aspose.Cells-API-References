---
title: "ChartDataTable.HasHorizontalBorder"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ChartDataTable 属性。如果图表数据表具有水平单元格边框，则为 True"
type: docs
url: /zh/net/aspose.cells.charts/chartdatatable/hashorizontalborder/
---
## ChartDataTable.HasHorizontalBorder property

如果图表数据表具有水平单元格边框，则为 True

```csharp
public bool HasHorizontalBorder { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyHasHorizontalBorderDemo
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

            // 设置图表数据源
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // 启用数据表
            chart.ShowDataTable = true;
            // 通过 ChartDataTable 属性获取数据表
            ChartDataTable dataTable = chart.ChartDataTable;

            // 演示 HasHorizontalBorder 属性
            dataTable.HasHorizontalBorder = true;
            Console.WriteLine("DataTable HasHorizontalBorder: " + dataTable.HasHorizontalBorder);

            // 保存工作簿
            workbook.Save("ChartDataTablePropertyHasHorizontalBorderDemo_out.xlsx");
        }
    }
}
```

### 另请参见

* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


