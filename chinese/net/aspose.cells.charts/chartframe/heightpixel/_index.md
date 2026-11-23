---
title: "ChartFrame.HeightPixel"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ChartFrame 属性。获取或设置框架的高度，单位为像素"
type: docs
url: /zh/net/aspose.cells.charts/chartframe/heightpixel/
---
## ChartFrame.HeightPixel property

获取或设置框架的高度，单位为像素。

```csharp
public virtual int HeightPixel { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyHeightPixelDemo
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
            
            // 向工作表添加图表
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // 设置图表数据源
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // 访问图表标题（它是一个 ChartFrame）
            ChartFrame chartTitle = chart.Title;
            
            // 显示当前高度（像素）
            Console.WriteLine("Current title height: " + chartTitle.HeightPixel + " pixels");
            
            // 为标题设置新的高度
            chartTitle.HeightPixel = 40;
            Console.WriteLine("New title height: " + chartTitle.HeightPixel + " pixels");
            
            // 访问图例（另一个 ChartFrame）
            ChartFrame legend = chart.Legend;
            
            // 显示并修改图例高度
            Console.WriteLine("Current legend height: " + legend.HeightPixel + " pixels");
            legend.HeightPixel = 60;
            Console.WriteLine("New legend height: " + legend.HeightPixel + " pixels");
            
            // 保存工作簿
            workbook.Save("ChartFrameHeightPixelDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


