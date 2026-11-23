---
title: "MsoFormatPicture.TopCropInch"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "MsoFormatPicture 属性。表示裁剪矩形顶部位置，以英寸为单位"
type: docs
url: /zh/net/aspose.cells.drawing/msoformatpicture/topcropinch/
---
## MsoFormatPicture.TopCropInch property

表示裁剪矩形顶部位置，以英寸为单位。

```csharp
public double TopCropInch { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyTopCropInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // 添加图片（替换为实际图像路径）
            int pictureIndex = sheet.Pictures.Add(0, 0, "sample.jpg");
            Aspose.Cells.Drawing.Picture picture = sheet.Pictures[pictureIndex];

            // 访问并修改 TopCropInch 属性
            Aspose.Cells.Drawing.MsoFormatPicture format = picture.FormatPicture;
            format.TopCropInch = 0.3; // Crop 0.3 inches from top
            format.BottomCropInch = 0.2; // Additional crop properties for context

            // 保存结果
            workbook.Save("TopCropInchDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


