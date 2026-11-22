---
title: "Picture.OriginalWidthInch"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Picture. تحصل على العرض الأصلي للصورة بوحدة البوصة"
type: docs
url: /ar/net/aspose.cells.drawing/picture/originalwidthinch/
---
## Picture.OriginalWidthInch property

يحصل على العرض الأصلي للصورة، بوحدة البوصة.

```csharp
public double OriginalWidthInch { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PicturePropertyOriginalWidthInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف صورة (استبدل "example.jpg" بمسار الصورة الفعلي الخاص بك)
            int imgIndex = worksheet.Pictures.Add(1, 1, "example.jpg");
            Picture pic = worksheet.Pictures[imgIndex];
            
            // احصل على العرض الأصلي وعرضه بوحدات البوصة
            double picWidthInch = pic.OriginalWidthInch;
            Console.WriteLine($"Original picture width: {picWidthInch} inches");
            
            workbook.Save("result.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


