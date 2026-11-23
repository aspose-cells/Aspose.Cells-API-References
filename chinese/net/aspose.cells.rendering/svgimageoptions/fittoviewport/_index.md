---
title: "SvgImageOptions.FitToViewPort"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SvgImageOptions 属性。如果此属性为 true，生成的 svg 将适配视口"
type: docs
url: /zh/net/aspose.cells.rendering/svgimageoptions/fittoviewport/
---
## SvgImageOptions.FitToViewPort property

如果此属性为 true，生成的 svg 将适配视口。

```csharp
public bool FitToViewPort { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Rendering;
    using System;

    public class SvgImageOptionsPropertyFitToViewPortDemo
    {
        public static void Run()
        {
            // 创建包含示例数据的新工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 填充单元格示例数据
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 150;
            worksheet.Cells["B3"].Value = 250;

            // 创建柱状图
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 18, 6);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            chart.Title.Text = "Sales Report";

            // 创建 SVG 渲染选项
            SvgImageOptions svgOptions = new SvgImageOptions();

            // 显示初始 FitToViewPort 值
            Console.WriteLine($"Initial FitToViewPort: {svgOptions.FitToViewPort}");

            // 修改属性并演示效果
            svgOptions.FitToViewPort = true;
            Console.WriteLine($"Modified FitToViewPort: {svgOptions.FitToViewPort}");

            // 使用不同设置将工作表渲染为 SVG
            SheetRender renderer = new SheetRender(worksheet, svgOptions);
            renderer.ToImage(0, "FitToViewPortEnabled.svg");

            // 可选：创建禁用 FitToViewPort 的对比
            svgOptions.FitToViewPort = false;
            renderer = new SheetRender(worksheet, svgOptions);
            renderer.ToImage(0, "FitToViewPortDisabled.svg");

            Console.WriteLine("Generated SVG files demonstrate FitToViewPort effect.");
        }
    }
}
```

### 另请参见

* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


