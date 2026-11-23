---
title: "RenderingWatermark.Font"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "RenderingWatermark 属性。获取水印的字体"
type: docs
url: /zh/net/aspose.cells.rendering/renderingwatermark/font/
---
## RenderingWatermark.Font property

获取水印的字体。

```csharp
public RenderingFont Font { get; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingWatermarkPropertyFontDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 创建渲染字体并设置初始属性
            RenderingFont font = new RenderingFont("Arial", 24);
            
            // 使用渲染字体创建文本水印
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font);
            
            // 显示初始字体属性
            Console.WriteLine("Initial Font Name: " + watermark.Font.Name);
            Console.WriteLine("Initial Font Size: " + watermark.Font.Size);
            Console.WriteLine("Initial Bold Status: " + watermark.Font.Bold);
            
            // 通过 RenderingFont 引用修改字体属性
            font.Bold = true;
            
            // 显示来自水印的更新后字体属性
            Console.WriteLine("\nUpdated Font Name: " + watermark.Font.Name);
            Console.WriteLine("Updated Font Size: " + watermark.Font.Size);
            Console.WriteLine("Updated Bold Status: " + watermark.Font.Bold);
            
            // 配置水印显示属性
            watermark.Opacity = 0.5f;
            watermark.Rotation = 45;
            watermark.IsBackground = true;
            
            // 创建 PDF 保存选项并分配水印
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.Watermark = watermark;
            
            // 保存带有水印 PDF 的工作簿以展示字体更改
            workbook.Save("RenderingWatermarkFontDemo.pdf", pdfSaveOptions);
        }
    }
}
```

### 另请参见

* class [RenderingFont](../../renderingfont/)
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


