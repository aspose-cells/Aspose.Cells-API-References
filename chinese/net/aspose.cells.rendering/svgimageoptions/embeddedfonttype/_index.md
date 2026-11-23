---
title: "SvgImageOptions.EmbeddedFontType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SvgImageOptions 属性。获取或设置嵌入在 Svg 中的字体类型"
type: docs
url: /zh/net/aspose.cells.rendering/svgimageoptions/embeddedfonttype/
---
## SvgImageOptions.EmbeddedFontType property

获取或设置嵌入到 Svg 中的字体类型。

```csharp
public SvgEmbeddedFontType EmbeddedFontType { get; set; }
```

### 备注

默认值为 None，表示它不会在 Svg 中嵌入字体。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SvgImageOptionsPropertyEmbeddedFontTypeDemo
    {
        public static void Run()
        {
            // 创建一个新工作簿并访问第一个工作表
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加带自定义格式的数据以演示字体嵌入
            var cell = worksheet.Cells["B2"];
            cell.PutValue("SVG Font Embedding Test");
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            cell.SetStyle(style);

            // 创建 SVG 渲染选项
            SvgImageOptions svgOptions = new SvgImageOptions();
            
            // 显示初始嵌入的字体类型
            Console.WriteLine($"Initial EmbeddedFontType: {svgOptions.EmbeddedFontType}");

            // 将工作表渲染为 SVG，且不嵌入字体
            SheetRender renderer = new SheetRender(worksheet, svgOptions);
            renderer.ToImage(0, "WithoutFontEmbedding.svg");

            // 将嵌入的字体类型更改为 WOFF
            svgOptions.EmbeddedFontType = SvgEmbeddedFontType.Woff;

            // 将工作表渲染为 SVG，并嵌入 WOFF 字体
            SheetRender renderer2 = new SheetRender(worksheet, svgOptions);
            renderer2.ToImage(0, "WithWoffFontEmbedding.svg");

            Console.WriteLine("Generated SVG files with different font embedding settings.");
        }
    }
}
```

### 另请参见

* enum [SvgEmbeddedFontType](../../svgembeddedfonttype/)
* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


