---
title: "ChartFrame.WidthPixel"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ChartFrame 属性。获取或设置以像素为单位的框宽度"
type: docs
url: /zh/net/aspose.cells.charts/chartframe/widthpixel/
---
## ChartFrame.WidthPixel property

获取或设置以像素为单位的框宽度。

```csharp
public virtual int WidthPixel { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyWidthPixelDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // 设置图表数据源
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // 访问图表标题（继承自 ChartFrame）
            chart.Title.Text = "Sample Chart";
            
            // 显示图表标题当前的 WidthPixel 值
            Console.WriteLine("Current Title WidthPixel: " + chart.Title.WidthPixel);
            
            // 以像素为单位为图表标题设置新的宽度
            chart.Title.WidthPixel = 300;
            
            // 显示新的 WidthPixel 值
            Console.WriteLine("New Title WidthPixel: " + chart.Title.WidthPixel);
            
            // 保存工作簿
            workbook.Save("ChartFrameWidthPixelDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


