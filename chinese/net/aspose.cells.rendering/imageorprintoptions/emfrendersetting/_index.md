---
title: "ImageOrPrintOptions.EmfRenderSetting"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ImageOrPrintOptions 属性。用于在源文件中渲染 EMF 元文件的设置"
type: docs
url: /zh/net/aspose.cells.rendering/imageorprintoptions/emfrendersetting/
---
## ImageOrPrintOptions.EmfRenderSetting property

用于在源文件中渲染 EMF 元文件的设置。

```csharp
public EmfRenderSetting EmfRenderSetting { get; set; }
```

### 备注

标识为 “EMF+ Dual” 的 EMF 元文件可以同时包含 EMF+ 记录和 EMF 记录。可以使用任意类型的记录来渲染图像，或仅使用 EMF+ 记录，或仅使用 EMF 记录。当设置 EmfPlusPrefer 时，渲染图像时将解析 EMF+ 记录；否则仅解析 EMF 记录。默认值为 EmfOnly。对于依赖 .NET System.Drawing.Common 的框架，此设置将被忽略。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing; // Added missing namespace AsposeCellsExamples
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyEmfRenderSettingDemo
    {
        public static void Run()
        {
            // 创建一个包含测试内容的新工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "EMF Rendering Setting Test";
            worksheet.Cells["C5"].Value = "Sample Content for Image Rendering";

            // 创建图像渲染选项
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Tiff;
            options.TiffCompression = TiffCompression.CompressionLZW;

            // 显示当前设置
            Console.WriteLine("Default EmfRenderSetting: " + options.EmfRenderSetting);

            // 使用默认的 EMF 设置进行渲染
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "DefaultEmfSetting.tiff");

            // 更改 EMF 渲染设置并重新渲染
            options.EmfRenderSetting = EmfRenderSetting.EmfPlusPrefer;
            Console.WriteLine("\nModified EmfRenderSetting: " + options.EmfRenderSetting);

            SheetRender modifiedRenderer = new SheetRender(worksheet, options);
            modifiedRenderer.ToImage(0, "ModifiedEmfSetting.tiff");

            Console.WriteLine("\nGenerated TIFF images demonstrating EMF rendering settings.");
        }
    }
}
```

### 另请参见

* enum [EmfRenderSetting](../../../aspose.cells/emfrendersetting/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


