---
title: "ImageOrPrintOptions.ChartImageType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ImageOrPrintOptions 属性。指示转换时的图表图像类型，默认值为 PNG"
type: docs
url: /zh/net/aspose.cells.rendering/imageorprintoptions/chartimagetype/
---
## ImageOrPrintOptions.ChartImageType property

指示转换时的图表图像类型，默认值：PNG。

```csharp
[Obsolete("Chart and Shape are always rendered as vector elements(e.g. point, line) for rendering quality.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ImageFormat ChartImageType { get; set; }
```

### 备注

注意：此成员已过时。相反，图表和形状始终渲染为矢量元素（例如点、线），以提升渲染质量。此属性将在自2022年6月起的12个月后移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class ImageOrPrintOptionsPropertyChartImageTypeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();

            // 添加一个包含图表的工作表
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["A2"].Value = 10;
            worksheet.Cells["A3"].Value = 20;
            worksheet.Cells["A4"].Value = 30;

            // 向工作表添加图表
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A2:A4", true);

            try
            {
                // 创建 ImageOrPrintOptions 实例
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // 显示当前的 ChartImageType 值
                Console.WriteLine("Current ChartImageType: " + options.ImageType);

                // 为图表渲染设置不同的图像类型
                options.ImageType = ImageType.Png;
                Console.WriteLine("ChartImageType set to: " + options.ImageType);

                // 创建 SheetRender 以演示该属性的效果
                SheetRender renderer = new SheetRender(worksheet, options);

                // 将图表渲染到内存流
                MemoryStream stream = new MemoryStream();
                renderer.ToImage(0, stream);

                Console.WriteLine("Chart rendered successfully with ChartImageType: " + options.ImageType);
                Console.WriteLine("Image size: " + stream.Length + " bytes");

                // 保存工作簿
                workbook.Save("ChartImageTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


