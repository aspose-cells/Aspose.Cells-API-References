---
title: "SvgImageOptions.ImageType"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SvgImageOptions 属性。获取或设置生成图像的格式，默认值为 PNG"
type: docs
url: /zh/net/aspose.cells.rendering/svgimageoptions/imagetype/
---
## SvgImageOptions.ImageType property

获取或设置生成图像的格式。默认值：PNG。

```csharp
public override ImageType ImageType { get; set; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SvgImageOptionsPropertyImageTypeDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 添加示例数据和图像
            worksheet.Cells["A1"].PutValue("Embedded Image Type Demonstration");
            int pictureIndex = worksheet.Pictures.Add(0, 1, "inputImage.png");
            Picture picture = worksheet.Pictures[pictureIndex];

            // 创建 SVG 渲染选项
            SvgImageOptions svgOptions = new SvgImageOptions();

            // 显示当前 ImageType（默认：PNG）
            Console.WriteLine("Current ImageType: " + svgOptions.ImageType);

            // 更改嵌入栅格图像的图像格式
            svgOptions.ImageType = ImageType.Jpeg;

            // 将工作表内容保存为不同图像格式的 SVG
            using (MemoryStream stream = new MemoryStream())
            {
                picture.ToImage(stream, svgOptions);
                File.WriteAllBytes("output_with_jpeg.svg", stream.ToArray());
            }

            // 重置为 PNG 格式
            svgOptions.ImageType = ImageType.Png;
            
            using (MemoryStream stream = new MemoryStream())
            {
                picture.ToImage(stream, svgOptions);
                File.WriteAllBytes("output_with_png.svg", stream.ToArray());
            }

            Console.WriteLine("SVG files created with different embedded image formats.");
        }
    }
}
```

### 另请参见

* enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


