---
title: "MsoFormatPicture.LeftCropInch"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "MsoFormatPicture 属性。表示裁剪矩形左侧位置，以英寸为单位"
type: docs
url: /zh/net/aspose.cells.drawing/msoformatpicture/leftcropinch/
---
## MsoFormatPicture.LeftCropInch property

表示裁剪矩形左侧位置，以英寸为单位。

```csharp
public double LeftCropInch { get; set; }
```

### 示例

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyLeftCropInchDemo
    {
        public static void Run()
        {
            // 创建工作簿
            var workbook = new Workbook();
            var sheet = workbook.Worksheets[0];

            // 加载图像数据
            byte[] imageData = File.ReadAllBytes("example.png");
            
            // 向工作表添加图片
            int pictureIndex = sheet.Pictures.Add(0, 0, new MemoryStream(imageData));
            var picture = sheet.Pictures[pictureIndex];

            // 设置并获取 LeftCropInch 属性
            picture.FormatPicture.LeftCropInch = 0.5;
            double leftCropValue = picture.FormatPicture.LeftCropInch;

            Console.WriteLine($"Left crop value in inches: {leftCropValue}");

            // 保存工作簿
            workbook.Save("LeftCropInchDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


