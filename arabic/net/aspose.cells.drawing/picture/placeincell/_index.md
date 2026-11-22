---
title: "Picture.PlaceInCell"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Picture. ضع هذه الصورة في الخلية"
type: docs
url: /ar/net/aspose.cells.drawing/picture/placeincell/
---
## Picture.PlaceInCell method

ضع هذه الصورة في الخلية

```csharp
[Obsolete("Use Picture.IsPlacedInCell property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void PlaceInCell()
```

### ملاحظات

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام الخاصية Picture.IsPlacedInCell. سيتم إزالة هذه الخاصية بعد 12 شهرًا اعتبارًا من يناير 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

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
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف صورة إلى ورقة العمل
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.png");
            Picture picture = worksheet.Pictures[pictureIndex];

            // ضع الصورة في الخلية A1
            picture.PlaceInCell();

            // تحقق من أن الصورة موضوعة في الخلية
            Cell cell = worksheet.Cells["A1"];
            byte[] imageData = cell.EmbeddedImage;
            Console.WriteLine("Image placed in cell A1. Image data length: " + imageData.Length);

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


