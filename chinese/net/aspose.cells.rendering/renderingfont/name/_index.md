---
title: "RenderingFont.Name"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "RenderingFont 属性。获取字体的名称"
type: docs
url: /zh/net/aspose.cells.rendering/renderingfont/name/
---
## RenderingFont.Name property

获取字体名称。

```csharp
public string Name { get; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingFontPropertyNameDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 创建 PDF 保存选项
            PdfSaveOptions options = new PdfSaveOptions();

            // 使用 "Arial" 创建初始渲染字体
            RenderingFont fontArial = new RenderingFont("Arial", 16);
            Console.WriteLine("Initial font name: " + fontArial.Name);

            // 使用初始字体创建水印
            RenderingWatermark watermark = new RenderingWatermark("Confidential", fontArial);
            watermark.Opacity = 0.5f;
            watermark.Rotation = 45;
            options.Watermark = watermark;

            // 使用初始字体水印保存
            workbook.Save("WatermarkInitial.pdf", options);

            // 使用 "Times New Roman" 创建新渲染字体
            RenderingFont fontTimesNewRoman = new RenderingFont("Times New Roman", 16);
            Console.WriteLine("\nModified font name: " + fontTimesNewRoman.Name);

            // 使用新字体更新水印
            RenderingWatermark updatedWatermark = new RenderingWatermark("Confidential", fontTimesNewRoman);
            updatedWatermark.Opacity = 0.5f;
            updatedWatermark.Rotation = 45;
            options.Watermark = updatedWatermark;

            // 使用修改后的字体水印保存
            workbook.Save("WatermarkModified.pdf", options);
        }
    }
}
```

### 另请参见

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


