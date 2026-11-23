---
title: "RenderingWatermark.Image"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "RenderingWatermark 属性。获取水印的图像"
type: docs
url: /zh/net/aspose.cells.rendering/renderingwatermark/image/
---
## RenderingWatermark.Image property

获取水印的图像。

```csharp
public byte[] Image { get; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System.IO;

    public class RenderingWatermarkPropertyImageDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 从文件加载图像数据
            byte[] originalImage = File.ReadAllBytes("watermark.png");

            // 使用初始图像创建基于图像的水印
            RenderingWatermark watermark = new RenderingWatermark(originalImage);
            Console.WriteLine("Initial image size: " + watermark.Image.Length + " bytes");

            // 修改水印属性
            watermark.Rotation = 45f;
            watermark.Opacity = 0.5f;
            watermark.ScaleToPagePercent = 75;
            watermark.IsBackground = true;
            watermark.HAlignment = TextAlignmentType.Center;
            watermark.VAlignment = TextAlignmentType.Center;

            // 创建带水印的 PDF 保存选项
            PdfSaveOptions pdfOptions = new PdfSaveOptions();
            pdfOptions.Watermark = watermark; // Fixed property name

            // 保存为带水印的 PDF 输出
            workbook.Save("WatermarkedOutput.pdf", pdfOptions);

            // 使用不同的图像创建新水印
            byte[] updatedImage = File.ReadAllBytes("updated_watermark.png");
            RenderingWatermark newWatermark = new RenderingWatermark(updatedImage);
            Console.WriteLine("Updated image size: " + newWatermark.Image.Length + " bytes");

            // 使用新水印保存
            pdfOptions.Watermark = newWatermark; // Fixed property name
            workbook.Save("UpdatedWatermark.pdf", pdfOptions);
        }
    }
}
```

### 另请参见

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


