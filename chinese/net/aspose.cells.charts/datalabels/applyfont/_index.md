---
title: "DataLabels.ApplyFont"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "DataLabels 方法。将数据标签的字体应用于所有子节点"
type: docs
url: /zh/net/aspose.cells.charts/datalabels/applyfont/
---
## DataLabels.ApplyFont method

将数据标签的字体应用于所有子节点。

```csharp
public void ApplyFont()
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataLabelsMethodApplyFontDemo
    {
        public static void Run()
        {
            // 创建工作簿并访问第一个工作表
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 为图表添加示例数据
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["A5"].PutValue("D");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // 向工作表添加图表
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // 设置图表数据源
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";
            
            // 显示数据标签
            Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;
            
            // 为数据标签设置新的字体颜色
            Color newColor = Color.Green;
            series.DataLabels.Font.Color = newColor;
            
            // 将字体设置应用于所有数据标签
            series.DataLabels.ApplyFont();
            
            // 保存工作簿
            workbook.Save("DataLabelsApplyFontDemo_out.xlsx");
        }
    }
}
```

### 另请参见

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


