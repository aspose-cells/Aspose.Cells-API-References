---
title: "RenderingFont.Size"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "RenderingFont 属性。获取以点为单位的字体大小"
type: docs
url: /zh/net/aspose.cells.rendering/renderingfont/size/
---
## RenderingFont.Size property

获取字体的点大小。

```csharp
public float Size { get; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingFontPropertySizeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // 创建初始字体并演示读取 Size 属性
            RenderingFont smallFont = new RenderingFont("Arial", 12);
            Console.WriteLine("Initial font size: " + smallFont.Size);

            // 使用初始字体大小创建水印
            PdfSaveOptions optionsSmall = new PdfSaveOptions
            {
                Watermark = new RenderingWatermark("CONFIDENTIAL", smallFont)
            };
            workbook.Save("SmallWatermark.pdf", optionsSmall);

            // 创建更大尺寸的新字体
            RenderingFont largeFont = new RenderingFont("Arial", 24);
            Console.WriteLine("Modified font size: " + largeFont.Size);

            // 创建具有更大字体大小的水印
            PdfSaveOptions optionsLarge = new PdfSaveOptions
            {
                Watermark = new RenderingWatermark("CONFIDENTIAL", largeFont)
            };
            workbook.Save("LargeWatermark.pdf", optionsLarge);
        }
    }
}
```

### 另请参见

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


