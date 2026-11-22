---
title: "Picture.ImageType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Picture. تحصل على تنسيق الصورة"
type: docs
url: /ar/net/aspose.cells.drawing/picture/imagetype/
---
## Picture.ImageType property

يحصل على تنسيق الصورة.

```csharp
public ImageType ImageType { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyImageTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إدراج الصورة الأولى (PNG)
            int imgIndex1 = worksheet.Pictures.Add(1, 1, "1.png");
            Picture pic1 = worksheet.Pictures[imgIndex1];
            Console.WriteLine("Picture 1 is of type: " + pic1.ImageType);

            // إدراج الصورة الثانية (JPEG)
            int imgIndex2 = worksheet.Pictures.Add(1, 9, "2.jpeg");
            Picture pic2 = worksheet.Pictures[imgIndex2];
            Console.WriteLine("Picture 2 is of type: " + pic2.ImageType);
        }
    }
}
```

### انظر أيضًا

* enum [ImageType](../../imagetype/)
* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


