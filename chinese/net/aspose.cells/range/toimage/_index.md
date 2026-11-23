---
title: "Range.ToImage"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Range 方法。将范围转换为图像"
type: docs
url: /zh/net/aspose.cells/range/toimage/
---
## Range.ToImage method

将范围转换为图像。

```csharp
public byte[] ToImage(ImageOrPrintOptions options)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| options | ImageOrPrintOptions | 将此范围转换为图像的选项 |

### 示例

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RangeMethodToImageWithImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // 从示例 Excel 文件创建工作簿
            Workbook workbook = new Workbook("example.xlsx");
            
            // 获取第一个工作表及其单元格
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // 创建范围 A1:J25
            Aspose.Cells.Range range = cells.CreateRange("A1:J25");
            
            // 创建图像选项
            ImageOrPrintOptions options = new ImageOrPrintOptions()
            {
                ImageType = Aspose.Cells.Drawing.ImageType.Png,
                HorizontalResolution = 300,
                VerticalResolution = 300
            };
            
            // 将范围转换为图像
            byte[] imageData = range.ToImage(options);
            
            // 将图像保存到文件
            File.WriteAllBytes("range_output.png", imageData);
        }
    }
}
```

### 另请参见

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


