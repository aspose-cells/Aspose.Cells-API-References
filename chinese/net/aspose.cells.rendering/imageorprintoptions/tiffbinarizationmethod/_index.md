---
title: "ImageOrPrintOptions.TiffBinarizationMethod"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ImageOrPrintOptions 属性。获取或设置在 ImageType 为 Tiff 且 TiffCompression 等于 Ccitt3 或 Ccitt4 时，将图像转换为 1 bpp 格式所使用的方法"
type: docs
url: /zh/net/aspose.cells.rendering/imageorprintoptions/tiffbinarizationmethod/
---
## ImageOrPrintOptions.TiffBinarizationMethod property

获取或设置在 [`ImageType`](../imagetype/) 为 Tiff 且 [`TiffCompression`](../tiffcompression/) 等于 Ccitt3 或 Ccitt4 时，将图像转换为 1 bpp 格式所使用的方法。

```csharp
public ImageBinarizationMethod TiffBinarizationMethod { get; set; }
```

### 备注

默认值为 FloydSteinbergDithering。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class ImageOrPrintOptionsPropertyTiffBinarizationMethodDemo
    {
        public static void Run()
        {
            // 创建包含示例数据的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 添加梯度数据以进行可视化演示
            for (int i = 0; i < 15; i++)
            {
                Cell cell = worksheet.Cells[i, 0];
                cell.PutValue(i * 7);
                Style style = cell.GetStyle();
                style.BackgroundColor = Color.FromArgb(i * 18, i * 18, i * 18);
                cell.SetStyle(style);
            }

            // 配置 TIFF 渲染选项
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Tiff,
                TiffCompression = TiffCompression.CompressionCCITT3,
                TiffColorDepth = ColorDepth.Format1bpp
            };

            // 显示当前的二值化方法
            Console.WriteLine("Initial TiffBinarizationMethod: " + options.TiffBinarizationMethod);

            // 使用默认阈值方法进行渲染
            new SheetRender(worksheet, options).ToImage(0, "ThresholdBinarization.tiff");

            // 切换为 Floyd-Steinberg 抖动
            options.TiffBinarizationMethod = ImageBinarizationMethod.FloydSteinbergDithering;
            Console.WriteLine("\nModified TiffBinarizationMethod: " + options.TiffBinarizationMethod);

            // 使用新方法进行渲染
            new SheetRender(worksheet, options).ToImage(0, "DitheringBinarization.tiff");

            Console.WriteLine("\nGenerated TIFF files demonstrate different 1bpp conversion methods.");
        }
    }
}
```

### 另请参见

* enum [ImageBinarizationMethod](../../imagebinarizationmethod/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


