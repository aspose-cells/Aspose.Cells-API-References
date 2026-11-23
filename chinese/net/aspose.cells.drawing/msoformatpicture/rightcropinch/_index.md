---
title: "MsoFormatPicture.RightCropInch"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "MsoFormatPicture 属性。表示裁剪矩形右侧位置，以英寸为单位"
type: docs
url: /zh/net/aspose.cells.drawing/msoformatpicture/rightcropinch/
---
## MsoFormatPicture.RightCropInch property

表示裁剪矩形右侧位置，以英寸为单位。

```csharp
public double RightCropInch { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyRightCropInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // 添加图片（替换为实际图像路径）
            int pictureIndex = sheet.Pictures.Add(1, 1, "sample.jpg");
            Aspose.Cells.Drawing.Picture picture = sheet.Pictures[pictureIndex];

            // 访问并设置 RightCropInch 属性
            Aspose.Cells.Drawing.MsoFormatPicture format = picture.FormatPicture;
            format.RightCropInch = 0.3; // Crop 0.3 inches from right

            // 保存工作簿
            workbook.Save("RightCropInchDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


