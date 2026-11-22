---
title: "Picture.OriginalWidthCM"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Picture. تحصل على العرض الأصلي للصورة بوحدة السنتيمتر"
type: docs
url: /ar/net/aspose.cells.drawing/picture/originalwidthcm/
---
## Picture.OriginalWidthCM property

يحصل على العرض الأصلي للصورة، بوحدة السنتيمتر.

```csharp
public double OriginalWidthCM { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyOriginalWidthCMDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpeg");
            Picture pic = worksheet.Pictures[imgIndex];
            
            Console.WriteLine("Original width of the picture in centimeters: " + pic.OriginalWidthCM);
            
            workbook.Save("result.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


