---
title: "RenderingWatermark.VAlignment"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "RenderingWatermark 属性。获取或设置水印相对于页面的垂直对齐方式"
type: docs
url: /zh/net/aspose.cells.rendering/renderingwatermark/valignment/
---
## RenderingWatermark.VAlignment property

获取或设置水印相对于页面的垂直对齐方式。

```csharp
public TextAlignmentType VAlignment { get; set; }
```

### 备注

仅支持 Top、Center、Bottom。默认是 Top。

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingWatermarkPropertyVAlignmentDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Watermark VAlignment Demo");

            // 创建 PDF 保存选项
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // 创建并配置具有不同 VAlignment 设置的水印
            RenderingFont font = new RenderingFont("Arial", 48)
            {
                Bold = true,
                Color = System.Drawing.Color.Red
            };

            // 创建垂直对齐设置为 Center 的水印
            RenderingWatermark watermark = new RenderingWatermark("CENTER ALIGNED", font)
            {
                VAlignment = TextAlignmentType.Center,
                HAlignment = TextAlignmentType.Center,
                Opacity = 0.5f
            };
            pdfSaveOptions.Watermark = watermark;

            // 将工作簿保存为带水印的文件
            workbook.Save("WatermarkVAlignmentDemo.pdf", pdfSaveOptions);
        }
    }
}
```

### 另请参见

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


