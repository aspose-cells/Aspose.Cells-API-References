---
title: "枚举 ImageBinarizationMethod"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Rendering.ImageBinarizationMethod 枚举。指定用于二值化图像的方法"
type: docs
url: /zh/net/aspose.cells.rendering/imagebinarizationmethod/
---
## ImageBinarizationMethod enumeration

指定用于二值化图像的方法。

```csharp
public enum ImageBinarizationMethod
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Threshold | `0` | 指定阈值方法。 |
| FloydSteinbergDithering | `1` | 指定使用 Floyd‑Steinberg 错误扩散法进行抖动。 |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class RenderingClassImageBinarizationMethodDemo
    {
        public static void Run()
        {
            // 创建一个包含测试数据的新工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 为演示填充带有渐变值的单元格
            for (int row = 0; row < 50; row++)
            {
                for (int col = 0; col < 10; col++)
                {
                    worksheet.Cells[row, col].PutValue((double)(row * col) / 500);
                }
            }

            // 配置图像渲染选项
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Tiff,
                TiffCompression = TiffCompression.CompressionCCITT4,
                TiffBinarizationMethod = ImageBinarizationMethod.FloydSteinbergDithering
            };

            // 使用配置的选项创建工作表渲染
            SheetRender renderer = new SheetRender(worksheet, options);
            
            // 将第一工作表页面渲染为带二值化的图像
            renderer.ToImage(0, "BinarizedOutput.tiff");
        }
    }
}
```

### 另请参见

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


