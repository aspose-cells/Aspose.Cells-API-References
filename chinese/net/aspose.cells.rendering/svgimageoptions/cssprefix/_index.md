---
title: "SvgImageOptions.CssPrefix"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SvgImageOptions 属性。获取和设置 svg 中 css 名称的前缀，默认值为空字符串"
type: docs
url: /zh/net/aspose.cells.rendering/svgimageoptions/cssprefix/
---
## SvgImageOptions.CssPrefix property

获取和设置 svg 中 css 名称的前缀，默认值为空字符串。

```csharp
public string CssPrefix { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SvgImageOptionsPropertyCssPrefixDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 为图表添加示例数据
            worksheet.Cells["A1"].PutValue("Year");
            worksheet.Cells["B1"].PutValue("Sales");
            
            worksheet.Cells["A2"].PutValue(2019);
            worksheet.Cells["A3"].PutValue(2020);
            worksheet.Cells["A4"].PutValue(2021);
            worksheet.Cells["A5"].PutValue(2022);

            worksheet.Cells["B2"].PutValue(4500);
            worksheet.Cells["B3"].PutValue(4900);
            worksheet.Cells["B4"].PutValue(5200);
            worksheet.Cells["B5"].PutValue(6100);

            // 创建折线图
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B5", true);

            // 创建 SVG 图像选项
            SvgImageOptions svgOptions = new SvgImageOptions();

            // 显示当前 CSS 前缀
            Console.WriteLine("Current CssPrefix value: " + svgOptions.CssPrefix);

            // 设置新的 CSS 前缀
            svgOptions.CssPrefix = "chart-prefix-";

            // 演示使用自定义 CSS 前缀的 SVG 生成
            string outputPath = "output_chart.svg";
            chart.ToImage(outputPath, svgOptions);

            Console.WriteLine("Chart saved as SVG with custom CSS prefix.");
        }
    }
}
```

### 另请参见

* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


