---
title: "RenderingWatermark.Text"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "RenderingWatermark 属性。获取水印的文本"
type: docs
url: /zh/net/aspose.cells.rendering/renderingwatermark/text/
---
## RenderingWatermark.Text property

获取水印的文本。

```csharp
public string Text { get; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingWatermarkPropertyTextDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 为水印文本创建渲染字体
            RenderingFont font = new RenderingFont("Arial", 36);

            // 使用字体配置初始化文本水印
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font);

            // 显示当前水印文本
            Console.WriteLine("Watermark Text: " + watermark.Text);

            // 配置水印外观
            watermark.Rotation = 45f;
            watermark.Opacity = 0.3f;
            watermark.IsBackground = true;
            watermark.ScaleToPagePercent = 150;

            // 将水印应用于 PDF 保存选项
            PdfSaveOptions options = new PdfSaveOptions();
            options.Watermark = watermark; // Fixed property name

            // 保存为 PDF 以可视化水印效果
            workbook.Save("WatermarkDemo.pdf", options);
        }
    }
}
```

### 另请参见

* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


