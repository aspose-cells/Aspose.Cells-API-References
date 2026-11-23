---
title: "MsoFormatPicture.BottomCropInch"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "MsoFormatPicture 属性。表示裁剪矩形底部位置，以英寸为单位"
type: docs
url: /zh/net/aspose.cells.drawing/msoformatpicture/bottomcropinch/
---
## MsoFormatPicture.BottomCropInch property

表示裁剪矩形底部位置，以英寸为单位。

```csharp
public double BottomCropInch { get; set; }
```

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyBottomCropInchDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // 向工作表添加图片（使用占位路径）
            int pictureIndex = sheet.Pictures.Add(5, 5, "sample.jpg");
            Picture picture = sheet.Pictures[pictureIndex];

            // 访问 MsoFormatPicture 对象
            MsoFormatPicture formatPicture = picture.FormatPicture;

            // 设置 BottomCropInch 属性并演示其用法
            formatPicture.BottomCropInch = 0.3;
            formatPicture.TopCropInch = 0.2;
            
            // 保存工作簿
            workbook.Save("MsoFormatPictureBottomCropDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


