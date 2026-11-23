---
title: "Picture.PlaceInCell"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Picture 方法。将此图片放置在单元格中"
type: docs
url: /zh/net/aspose.cells.drawing/picture/placeincell/
---
## Picture.PlaceInCell method

将此图片放入单元格中

```csharp
[Obsolete("Use Picture.IsPlacedInCell property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void PlaceInCell()
```

### 备注

注意：此成员现已过时。请改用 Picture.IsPlacedInCell 属性。此属性将在自 2026 年 1 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

### 示例

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PictureMethodPlaceInCellDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 向工作表添加图片
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.png");
            Picture picture = worksheet.Pictures[pictureIndex];

            // 将图片放置在单元格 A1 中
            picture.PlaceInCell();

            // 验证图片已放置在单元格中
            Cell cell = worksheet.Cells["A1"];
            byte[] imageData = cell.EmbeddedImage;
            Console.WriteLine("Image placed in cell A1. Image data length: " + imageData.Length);

            // 保存工作簿
            workbook.Save("output.xlsx");
        }
    }
}
```

### 另请参见

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


